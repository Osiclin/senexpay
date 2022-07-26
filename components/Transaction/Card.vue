<template>
    <div class="card">
        <div>
            <div class="icon"><slot/></div>
            <p class="para">{{ title }}</p>
        </div>
        <div>
            <div>
                <p class="amount">${{ buy_amount }}</p>
                <Button radius="4px" bgcolor="#049642" color="#ffffff">
                    Buy
                </Button>
            </div>
            <div>
                <p class="amount">${{ sell_amount }}</p>
                <Button radius="4px" bgcolor="#FF5F24" color="#ffffff">
                    Sell
                </Button>
            </div>
        </div>
    </div>
</template>

<script>
import Button from '../Button.vue'

export default {
    name: 'NuxtCard',
    components: { Button },
    props: ['title', 'sell_amount', 'buy_amount']
}
</script>

<style scoped>
.card{
    display: flex;
    max-width: 1200px;
    margin: 0 auto 1rem;
    background-color: #041D45;
    padding: 1rem;
    border-radius: 10px;
}
.card>div{
    display: flex;
    align-items: center;
}
.card>div:first-child{
    flex: .6;
}
.card>div:last-child{
    flex: .4;
}
.card>div:last-child>div{
    display: flex;
    align-items: center;
}
.card>div:last-child>div:first-child{
    margin-right: 1rem;
}
.icon{
    margin-right: .5rem;
}
.amount{
    margin-right: 1rem;
    font-size: 1.575rem;
    font-family: SF Pro Bold;
}
.para{
    font-size: 1.575rem;
}
@media screen and (max-width: 900px) {
    .card>div:last-child{
        display: flex;
        flex-direction: column;
    }
    .card>div:last-child>div:first-child{
        margin-right: 0;
    }
}
</style>