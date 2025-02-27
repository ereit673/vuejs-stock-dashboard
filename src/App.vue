<template>
  
    <BaseCard></BaseCard>
  
</template>

<script>
import BaseCard from './components/BaseCard.vue';
import { stockService } from '@/services/stockService';

export default {
  name: 'App',
  components: {
    BaseCard
  },
  async created() {
    this.data = await stockService.getRevenue('$AAPL');
    console.log('Loaded data', this.data);
  }
}
</script>

<style>
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body{
  background: radial-gradient(71.11% 100% at 50% 0%, #020204 14.6%, #011F35 100%);
}

#app {
  padding: 100px;
  width:100%;
  min-height: 100dvh;
}
</style>
