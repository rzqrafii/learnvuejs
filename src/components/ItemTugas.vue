<template>
  <div>
    <input class="form-check-input" type="checkbox" value id="defaultCheck1" />
    <label
      class="form-check-label item"
      v-bind:class="{'item-completed':tugasSaya.isDone}"
      for="defaultCheck1"
    >{{tugasSaya.namaTugas}}</label>
  </div>
</template>

<script>
export default {
    // props akan dipanggil pada app.vue (daftar props)
    name:"ItemTugas",
    props:["tugasSaya"]
};
</script>

<style scoped>
</style>
