<template>
  <header class="py-4">
    <div class="flex justify-between">

      <div class="flex items-center">
        <img class="w-12" src="@/assets/purple-logo.png" alt="logo">
        <div class="ml-2 text-xl">MyTube</div>
      </div>

      <div class="w-3/5">
        <search-video @enterVideos="getVideo"/>
      </div>
      <profile-picture/>

    </div>

  </header>

<!--  <div v-for="video of videos">-->
<!--    <div>{{video.title}}</div>-->
<!--  </div>-->

</template>

<script>

import ProfilePicture from "@/components/UI/ProfilePicture.vue";
import SearchVideo from "@/components/SearchVideo.vue";

export default {
    components: {
        ProfilePicture, SearchVideo
    },
    data() {
        return {
            videos: []
        }
    },
    methods: {
        getVideo(data) {
            // console.log(data)
            this.videos = data
        }
    }

}
</script>

<style lang="scss" scoped>

</style>