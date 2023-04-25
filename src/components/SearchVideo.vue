<template>
  <div class="flex">
    <div class="relative w-full">
      <input v-model="search"
             class="w-full h-full border px-6 py-2 rounded-l-full text-lg"
             type="text"
             placeholder="Search"
             @input="searchVideo"
      >
      <div class="absolute top-1/2 -translate-x-1/2 -translate-y-1/2 right-0.5">
        <close-icon/>
      </div>
    </div>


    <div class="border px-8 rounded-r-full bg-gray-100 relative ">
      <img class="w-6 absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 cursor-pointer"
           src="@/assets/search.png" alt="search">
    </div>
  </div>
</template>

<script>
import CloseIcon from "@/components/UI/CloseIcon.vue";

export default {
    components: {CloseIcon},
    data() {
        return {
            search: '',
            videos: [
                {
                    title: 'Видео про VueJs'
                },
                {
                    title: 'Видео про Angular'
                },
                {
                    title: 'Видео про React'
                },
                {
                    title: 'Видео про Tailwind'
                },
            ]
        }
    },
    methods: {
        searchVideo() {
            const text_value = this.search
            const result = this.videos.filter(video =>
                video.title.includes(text_value)) //перебор массива и поиск совпадений
            this.$emit ('enterVideos', result)
        }
    }
}
</script>

<style lang="scss" scoped>

</style>