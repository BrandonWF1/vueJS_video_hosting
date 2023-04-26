<template>
  <div class="xl:w-4/5 flex xl:flex-row flex-col items-center xl:items-start mb-10">
    <div class="w-3/4 xl:px-5 max-w-xl hover:scale-105 duration-300"><img class="rounded-2xl" :src="video.preview" alt=""></div>
    <div class="flex flex-col xl:w-1/2 w-3/4">
      <div class="xl:text-4xl text-2xl py-2 font-medium overflow-hidden">{{video.title}}</div>
      <div class="text-gray-500 text-sm overflow-hidden py-1 flex flex-row items-center">
        <p>{{video.date}}</p>
        <div class="bg-gray-500 w-1 h-1 mx-2 rounded-full"></div>
        <p>{{video.views}} views</p>
      </div>
      <div class="flex items-center py-2">
        <div class="w-6 h-6 rounded-full border bg-gray-200 cursor-pointer mr-3"></div>
        <span class="text-gray-500 text-sm font-bold xl:font-normal overflow-hidden">{{video.author}}</span>
      </div>
      <div class="text-gray-600 xl:text-md text-sm">
        {{video.description}}
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
      video: {
          type: Object,
          required: true
      }
  },
}
</script>

<style lang="scss" scoped>

</style>