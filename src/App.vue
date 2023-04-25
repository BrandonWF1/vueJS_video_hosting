<template>

  <div class="container mx-auto">
    <header-component/>


    <main class="py-5">

      <section class="w-4/5 mx-auto">
        <div class="mb-2 flex flex-row items-center font-bold cursor-pointer">
          <img class="w-7 mr-1" src="@/assets/filters.png" alt="filters">
          <span>Filters</span>
        </div>
        <hr class="mb-5">


        <div class="w-4/5 flex mb-10">
          <div class="w-1/2 px-5"><img class="rounded-2xl" src="@/assets/preview.jpg" alt=""></div>
          <div class="flex flex-col w-1/2">
            <div class="text-4xl py-2 font-medium overflow-hidden">synthwave radio 🌌 - beats to chill/study</div>
            <div class="text-gray-500 text-sm overflow-hidden py-1 flex flex-row items-center">
              <p>2 Days ago</p>
              <div class="bg-gray-500 w-1 h-1 mx-2 rounded-full"></div>
              <p>123K Views</p>
            </div>
            <div class="flex items-center py-2">
              <div class="w-6 h-6 rounded-full border bg-gray-200 cursor-pointer mr-3"></div>
              <span class="text-gray-500 text-sm overflow-hidden">Author</span>
            </div>
            <div class="text-gray-600">Insert Description of video here. Lorem ipsum dolor sit amet, consectetur adipisicing elit. Repellat, sit!</div>
          </div>
        </div>

        <div class="w-4/5 flex mb-10">
          <div class="w-1/2 px-5"><img class="rounded-2xl" src="@/assets/preview3.jpg" alt=""></div>
          <div class="flex flex-col w-1/2">
            <div class="text-4xl py-2 font-medium overflow-hidden">Retro Wave mix - Black Cat Audio</div>
            <div class="text-gray-500 text-sm overflow-hidden py-1 flex flex-row items-center">
              <p>2 Days ago</p>
              <div class="bg-gray-500 w-1 h-1 mx-2 rounded-full"></div>
              <p>123K Views</p>
            </div>
            <div class="flex items-center py-2">
              <div class="w-6 h-6 rounded-full border bg-gray-200 cursor-pointer mr-3"></div>
              <span class="text-gray-500 text-sm overflow-hidden">Author</span>
            </div>
            <div class="text-gray-600">Insert Description of video here. Lorem ipsum dolor sit amet, consectetur adipisicing elit. Repellat, sit!</div>
          </div>
        </div>

        <div class="w-4/5 flex mb-10">
          <div class="w-1/2 px-5"><img class="rounded-2xl" src="@/assets/preview2.jpg" alt=""></div>
          <div class="flex flex-col w-1/2">
            <div class="text-4xl py-2 font-medium overflow-hidden">lofi hip hop radio 📚 - beats to relax/study to</div>
            <div class="text-gray-500 text-sm overflow-hidden py-1 flex flex-row items-center">
              <p>2 Days ago</p>
              <div class="bg-gray-500 w-1 h-1 mx-2 rounded-full"></div>
              <p>123K Views</p>
            </div>
            <div class="flex items-center py-2">
              <div class="w-6 h-6 rounded-full border bg-gray-200 cursor-pointer mr-3"></div>
              <span class="text-gray-500 text-sm overflow-hidden">Author</span>
            </div>
            <div class="text-gray-600">Insert Description of video here. Lorem ipsum dolor sit amet, consectetur adipisicing elit. Repellat, sit!</div>
          </div>
        </div>

      </section>

    </main>
  </div>
</template>

<script>
import HeaderComponent from '@/components/HeaderComponent.vue'

export default {
    components: {
        HeaderComponent
    },
    data() {
        return {}
    }
}
</script>

<style lang="scss">

</style>