<template>
  <div>
    <Hero/>
    <Transactions/>
    <Trust/>
  </div>
</template>

<script>
import Transactions from '../components/Transaction/Transactions.vue'
import Hero from '../components/Hero.vue'
import Trust from '../components/Trust/Trust.vue'

export default {
  name: 'IndexPage',
  components: {
    Transactions,
    Hero,
    Trust
}
}
</script>