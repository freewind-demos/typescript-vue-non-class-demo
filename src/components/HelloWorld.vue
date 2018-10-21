<template>
  <div class="hello">
    <div>
      <input type="text" v-model="message"/>
      <button @click="alertMessage">Alert</button>
    </div>
    <div>
      {{ message }}
    </div>
  </div>
</template>

<script lang="ts">
  import Vue from 'vue'

  export default Vue.extend({
    props: ['msg'],
    data: function () {
      return {
        message: this.msg
      }
    },
    methods: {
      alert: function (text: string) {
        window.alert(text)
      },
      alertMessage: function () {
        this.alert(this.message);
      }
    }
  })
</script>

<style scoped>
  .hello {
    color: red;
  }
</style>
