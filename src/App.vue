<template>
  <div id="app">
    <input type="text" v-on:input="cssClass = $event.target.value" >
    <p v-bind:class="cssClass">Class: {{ cssClass }}</p>
  </div>
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      cssClass: ''
    }
  }
}
</script>

<style lang="scss">
#app {

  p {
    background: grey;
  }

  .red {
    background: red;
    padding: 1rem;
  }
  .blue {
    background: blue;
    padding: 1rem;
  }

}
</style>
