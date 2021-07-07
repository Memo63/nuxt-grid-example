<template>
  <div>
    <Grid
      :source="trails"
    />
  </div>
</template>

<script>
const { trails } = require('~/trails')

export default {
  data () {
    return { trails }
  }

}
</script>

<style>

</style>
