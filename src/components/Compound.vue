<template>
  <div class="compound">
    <h1>Compound Working</h1>
    {{ Cii }}
    {{ Ctime}}
  </div>
</template>

<script>
export default {
  props: {
    Cii: Number,
    Ctime: Number
  }
}
</script>
