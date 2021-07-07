<template>
  <div class="mx-10 md:mx-24 mb-8 mt-16">
    <div class="mt-10 mb-12 relative ">
      <p class="uppercase text-lg md:text-xl w-48 md:w-full">
        for every girl and every grandpa
      </p>
      <p class="uppercase text-lg md:text-6xl w-48 md:w-full">
        asdfasdf
      </p>
      <p class="uppercase text-4xl md:text-5xl w-60 md:w-full font-bold mt-8">
        Wexl Trails erleben
      </p>
    </div>
    <div class="grid grid-cols-1 md:grid-cols-2 relative gap-8">
      <Card
        v-for="(item, index) in source"
        :key="index"
        :sub-item="item"
        :class="{'md:row-span-2': index===0}"
      >
        <template #action>
          <button type="button" class="uppercase bottom-10 left-10 absolute text-left p-1 font-medium w-40 bg-gray-600">
            mehr erfahren
          </button>
        </template>
      </Card>
      <button type="button" class="rounded-full rotate-12 md:h-28 md:w-28 h-14 w-14 text-xs md:text-lg text-center uppercase  top-0 right-0 absolute p-1  bg-gray-600 transform -translate-y-3/4 translate-x-1/4">
        ticket buchen
      </button>
    </div>
  </div>
</template>

<script>

export default {
  props: {
    source: {
      type: Array,
      default: () => []
    }
  }
}
</script>

<style lang="postcss" scoped>

</style>
