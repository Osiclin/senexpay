<template>
    <div class="container">
        <div class="wrapper">
            <div>
                <h2 class="title">Your trusted<br/>crypto exchange</h2>
                <p class="para">Our fast payout is why people trust us. Skip the long waits and join the cool people who use SenexPay to buy and sell cryptocurrency everyday.</p>
            </div>
            <div>
                <div>
                    <div class="circle">
                        <IconCircle/>
                    </div>
                    <div class="sa bubble">
                        <IconSABubble/>
                    </div>
                    <div class="nigeria bubble">
                        <IconNigeriaBubble/>
                    </div>
                    <div class="ghana bubble">
                        <IconGhanaBubble/>
                    </div>
                    <div class="appScreen2">
                        <img src="../../static/images/App_screen2.png" width="100%" height="100%" alt="app screen" />
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import IconCircle from "../icons/IconCircle.vue";
import IconSABubble from "../icons/IconSABubble.vue";
import IconNigeriaBubble from "../icons/IconNigeriaBubble.vue";
import IconGhanaBubble from "../icons/IconGhanaBubble.vue";

export default{
    name: 'NuxtTrust',
    components: { 
        IconCircle, 
        IconSABubble, 
        IconNigeriaBubble, 
        IconGhanaBubble 
    }
}
</script>

<style scoped>
.container{
    padding: 3rem 2rem;
}
.wrapper{
    min-height: 550px;
    max-width: 1400px;
    margin: 0 auto;
    display: flex;
}
.wrapper>div:first-child {
    display: flex;
    width: 800px;
    flex-direction: column;
    justify-content: center;
    margin-right: 1rem;
}
/* .wrapper>div:last-child {
    width: 900px;
    display: flex;
    justify-content: center;
    position: relative;
} */
.wrapper>div:last-child>div {
    height: 600px;
    width: 700px;
    margin: 0 auto;
    display: flex;
    justify-content: center;
    position: relative;
}
.title{
    font-size: 4.075rem;
    color: #053888;
}
.para{
    max-width: 579px;
    letter-spacing: 0px;
    color: #3E3E41;
    opacity: 1;
    font-size: 1.575rem;
}
.circle{
    width: 359px;
}
.appScreen2{
    position: absolute;
    top: 50px;
    max-width: 359px;
}
.bubble{
    position: absolute;
    left: 0;
    z-index: 1;
}
.sa{
    top: 230px;
}
.nigeria{
    top: 160px;
}
.ghana{
    top: 300px;
}

@media screen and (max-width: 1100px) {
  .wrapper{
    flex-wrap: wrap;
  }
  .wrapper>div:first-child {
    text-align: center;
    margin: 4rem 0;
    width: 100%;
    }
    .wrapper>div:last-child {
        width: 100%;
    }
    .para{
        max-width: 600px;
        margin: 0 auto;
    }
}
@media screen and (max-width: 600px) {
    .wrapper>div:last-child>div {
        height: 600px;
        width: 100%;
    }
}
</style>