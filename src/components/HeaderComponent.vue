<template>
  <header class="py-4">
    <div class="flex md:justify-between flex-wrap md:flex-nowrap">

      <div class="flex items-center order-1 mx-auto md:mx-0">
        <img class="w-12" src="@/assets/purple-logo.png" alt="logo">
        <div class="ml-2 text-md">MyTube</div>
      </div>

      <div class="md:w-3/5 w-4/5 mx-auto md:m-0 pt-3 md:order-1 order-3">
        <search-video :videos="videos" @enterVideos="getVideo"/>
      </div>

      <profile-picture class=" md:order-1 order-2 mx-auto md:mx-0" />

    </div>

  </header>


</template>

<script>

import ProfilePicture from "@/components/UI/ProfilePicture.vue";
import SearchVideo from "@/components/SearchVideo.vue";

export default {
    components: {
        ProfilePicture, SearchVideo
    },
    props: {
        videos: {
            type: Array,
            required: true
        }
    },
    data() {
        return {
        }
    },
    methods: {
        getVideo(data) {
            this.$emit ("findVideos", data)
        }
    }

}
</script>

<style lang="scss" scoped>

</style>