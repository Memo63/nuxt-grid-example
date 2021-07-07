<template>
  <Slots>
    This text is applied to the default slot.
    <template #second>
      <p>
        This is applied to the second slot.
      </p>
    </template>
    <template #third>
      <p>
        This is applied to the third slot.
      </p>
    </template>
  </Slots>
</template>

<script>
export default {

}
</script>

<style lang="postcss" scoped>

</style>
