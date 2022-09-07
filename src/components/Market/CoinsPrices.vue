<template>
    <div class="coin-market">
      <div class="row">
        <h1>Coin Market</h1>
        <input type="text" placeholder="Search" class="search" v-model="textSearch" @keyup="searchCoin()"/>
        <div class="table">
            <table>
                <thead>
                    <tr>
                        <th v-for="(title) in titles">
                            {{ title }}
                        </th>
                    </tr>
                </thead>
                <tbody>
                    <tr v-for="(coin) in filteredCoins" :key="coin.id">
                        <td>
                            <img :src="coin.image" :alt="coin.name" class="coin-img" />
                            <span>
                            {{ coin.name }}
                            </span>
                            <span>
                            {{ coin.symbol }}
                            </span>
                        </td>
                        <td>${{ coin.current_price.toLocaleString() }}</td>
                        <td>{{ coin.total_volume.toLocaleString() }}</td>
                    </tr>
                </tbody>
            </table>
        </div>
      </div>
    </div>
</template>
  
<script>
  export default {
    data() {
      return {
        coins: [],
        filteredCoins: [],
        titles: ["Coin", "Price", "24h Volume"],
        textSearch: "",
      };
    },
    async mounted() {
      const res = await fetch("https://api.coingecko.com/api/v3/coins/markets?vs_currency=usd&order=market_cap_desc&per_page=100&page=1&sparkline=false");
      const data = await res.json();
      this.coins = data;
      this.filteredCoins = data;
    },
    methods: {
      searchCoin() {
        this.filteredCoins = this.coins.filter(
          (coin) =>
            coin.name.toLowerCase().includes(this.textSearch.toLowerCase()) ||
            coin.symbol.toLowerCase().includes(this.textSearch.toLowerCase())
        );
      },
    },
  };
</script>
  
<style scoped>
.coin-market{
    text-align: center;
    padding: 20px;
    font-family: 'telex', sans-serif;
}
.table{
    padding: 10px;
    padding-left: 80px;
    width:450px;
    height: 400px;
    position: fixed;
    left: 50%;
    top: 50%;
    transform: translate(-50%, -50%);
    border-radius:10px;
    background:#fff;
    box-shadow: 2px 1px 21px -9px rgba(0,0,0,0.38);
    overflow: scroll;
}
.table::-webkit-scrollbar{
    display: none;
}
.coin-img{
    width: 2rem;
}
</style>