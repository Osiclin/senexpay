<template>
  <div class="container">
    <Navbar/>
    <div class="hero">
      <div>
        <h1 class="heroText">Buy and Sell <span class="focus">Crypto</span> the easier way.</h1>
        <p>SenexPay created the simplest way to buy and sell Bitcoin and USDT in minutes.</p>
        <div class="storeDiv">
          <Button color="#064EBE" radius="120px">
            <IconApple/>
            <span>App Store</span>
          </Button>
          <Button color="#064EBE" radius="120px">
            <IconGoogle/>
            <span>Google Play</span>
          </Button>
        </div>
      </div>
      <div>
        <div class="imgAppDiv">
          <img src="../static/images/App_home_screen.png" width="100%" height="100%" alt="app" />
        </div>
        <div class="imgWidgetDiv">
          <div class="stat">
            <img src="../static/images/dashboard_widget1.png" width="100%" height="100%" alt="widget" />
          </div>
          <div class="stat">
            <img src="../static/images/dashboard_widget2.png" width="100%" height="100%" alt="widget" />
          </div>
          <div class="baseDiv">
            <IconEasy/>
            <IconSwift/>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Navbar from './Navbar.vue';
import Button from './Button.vue';
import IconApple from './icons/IconApple.vue';
import IconGoogle from './icons/IconGoogle.vue';
import IconEasy from './icons/IconEasy.vue';
import IconSwift from './icons/IconSwift.vue';
import IconEasy1 from './icons/IconEasy.vue';

export default {
    name: "NuxtHero",
    components: { Navbar, Button, IconApple, IconGoogle, IconEasy, IconSwift, IconEasy1 }
}
</script>

<style scoped>
.container{
  width: 100%;
  background: #041D45;
}
.hero{
  min-height: 100vh;
  padding: 10rem 2rem 3rem;
  display: flex;
  max-width: 1400px;
  margin: 0 auto;
}
.heroText{
  font-family: SF Pro Bold;
  font-size: 4.7rem;
}
.hero>div:first-child{
  max-width: 750px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  margin-right: 2rem;
}
.hero>div:last-child{
  display: flex;
  max-height: 530px;
  flex-shrink: 0;
}
.hero>div:first-child>p{
  max-width: 700px;
  font-size: 1.575rem;
}
.focus{
  background: transparent linear-gradient(109deg, #1265FB 0%, #00FFFF 100%) 0% 0% no-repeat padding-box;
  background-clip: text;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
.imgAppDiv{
  max-width: 359px;
  height: 100%;
  margin-right: 2rem;
}
.imgWidgetDiv{
  width: 300px;
  height: 100%;
}
.storeDiv{
  display: flex;
}
.storeDiv>button:first-child{
  margin-right: 1rem;
}
.baseDiv{
  display: flex;
  align-items: center;
}
.baseDiv>svg:first-child{
  margin-right: 1rem;
}
.stat{
  height: 209px;
  margin-bottom: 2rem;
}

@media screen and (max-width: 1100px) {
  .hero{
    flex-wrap: wrap;
  }
  .hero>div:first-child{
    max-width: 800px;
    margin: 2rem auto 3rem;
    text-align: center;
    align-items: center;
  }
  .hero>div:first-child>p{
    max-width: 600px;
  }
  .hero>div:last-child{
    width: 100%;
    justify-content: center;
    flex-shrink: unset;
    margin-top: 0;
  }
  .stat{
    height: auto;
  }
}

@media screen and (max-width: 600px) {
  .hero>div:last-child{
    height: auto;
  }
}
</style>
