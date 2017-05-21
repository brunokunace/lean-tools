<template>
  <q-layout class="layout-padding">
    <div>
      <q-numeric
        v-model="number"
        :min="0"
        :max="1000"
        :step="10"
      ></q-numeric>
    </div>
  </q-layout>
</template>

<script>
export default {
  data () {
    return {
      number: 0
    }
  }
}
</script>

<style>
</style>
