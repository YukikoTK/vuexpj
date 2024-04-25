<template>
  <div id="app">
    <button @click="increase">増加</button>
    <p>{{ $store.state.count }}</p>
  </div>
</template>

<script>
export default {
  methods: {
    increase () {
      this.$store.dispatch('incrementAction');
    }
  }
}
</script>

<style>

</style>
