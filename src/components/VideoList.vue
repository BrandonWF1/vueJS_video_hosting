<template>
  <section class="max-w-5xl mx-auto">
    <div class="mb-2 flex flex-row items-center font-bold cursor-pointer">
      <img class="w-7 mr-1" src="@/assets/filters.png" alt="filters">
      <span>Filters</span>
    </div>
    <hr class="mb-5">

    <video-item v-for="video in videos" :video="video"/>

  </section>
</template>

<script>
import VideoItem from "@/components/VideoItem.vue";
export default {
    components: {
        VideoItem
    },
    props: {
        videos: {
            type: Array,
            required: true
        }
    }
}
</script>

<style lang="scss" scoped>

</style>