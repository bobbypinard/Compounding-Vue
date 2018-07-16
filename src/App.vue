<template>
  <div id="app">

    <form action="">
      <label for="ii">Initial Investment</label>
      <input v-model="ii" type="number" id="ii" /><br />
      <label for="compounded">Compounded</label>
      <input v-model="time" type="number" id="time" /><br />
      <input type="submit" text="Submit" />
      {{ ii * time }}
    </form>

    <compound :Cii="ii" :Ctime="time" />
  </div>
</template>

<script>
import Compound from "./components/Compound"

export default {
  components: {
    Compound
  },
  name: 'app',
  data () {
    return {
      ii: 0,
      time: 0
    }
  }
}
</script>

<style lang="scss">
input {
  width: 5em;
}
</style>
