<template>
  <div>
    <h1>App</h1>
    <HelloWorld/>
  </div>
</template>

<script lang="ts">
  import HelloWorld from './components/HelloWorld.vue';
  import Vue from 'vue';
  export default Vue.extend({
    components: {
      HelloWorld
    }
  })
</script>
