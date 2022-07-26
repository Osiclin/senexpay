<template>
    <div class="container">
        <Card title="Bitcoin" buy_amount="4,7842.00" sell_amount="4,7842.00">
            <IconBitcoin/>
        </Card>
        <Card title="USDT" buy_amount="4,7842.00" sell_amount="4,7842.00">
            <IconTether/>
        </Card>
        <Card title="DOGE COIN" buy_amount="4,7842.00" sell_amount="4,7842.00">
            <IconTether/>
        </Card>
        <p>SenexPay Transaction fee is 0.7 percent pegged at $2. <nuxt-link to="/" class="learn">Learn more</nuxt-link> about our fees.</p>
    </div>
</template>

<script>
import Card from './Card.vue';
import IconBitcoin from '../icons/IconBitcoin.vue';
import IconTether from '../icons/IconTether.vue';

export default {
    name: "NuxtTransactions",
    components: { Card, IconBitcoin, IconTether }
}
</script>

<style scoped>
.container{
    background-color: #042B69;
    padding: 5rem 1rem;
}
.container>p{
    margin: 3rem 0 0;
    text-align: center;
    font-size: 1.875rem;
}
.learn{
    color: #5694FC;
}
</style>