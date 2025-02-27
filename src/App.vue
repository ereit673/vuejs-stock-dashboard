<template>
  
    <BaseCard></BaseCard>
  
</template>

<script>
import BaseCard from './components/BaseCard.vue';


export default {
  name: 'App',
  components: {
    BaseCard
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
