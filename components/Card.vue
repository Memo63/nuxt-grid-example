<template>
  <div class="relative text-white">
    <div class="relative aspect-w-16 aspect-h-9 md:h-full">
      <img class="mx-auto absolute" src="https://picsum.photos/600/400">
    </div>
    <p class="text-3xl absolute font-bold left-10 bottom-20 uppercase">
      {{ subItem.title }}
    </p>
    <slot name="action" />
  </div>
</template>

<script>

export default {
  props: {
    subItem: {
      type: Object,
      default: () => {}
    }
  }

}

</script>

<style lang="postcss" scoped>

</style>
