<template>
  <div class="pt-24">
    <div class="container px-3 mx-auto flex flex-wrap flex-col md:flex-row items-center">
      <!--Left Col-->
      <div
        class="flex flex-col w-full md:w-2/5 justify-center items-start text-center md:text-left"
      >
        <p class="uppercase tracking-loose w-full">Metric Display</p>
        <h1 class="my-4 text-5xl font-bold leading-tight">つながるダッシュボード</h1>
        <p class="leading-normal text-2xl mb-8">ソーシャルネットワークからインターネット家電まで美しく表示</p>

        <a
          class="mx-auto lg:mx-0 hover:underline bg-white text-gray-800 font-bold rounded-full my-6 py-4 px-8 shadow-lg"
          v-bind:href="this.$constant.app_url"
        >使ってみる</a>
      </div>
      <!--Right Col-->
      <div class="w-full md:w-3/5 py-6 text-center">
        <img class="w-full md:w-4/5 z-50" :src="heroImage" alt />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data: function() {
    return {
      heroImage: '/hero.png'
    }
  }
}
</script>
