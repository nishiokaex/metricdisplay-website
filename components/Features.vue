<template>
  <section class="bg-white border-b py-8">
    <div class="container max-w-5xl mx-auto m-8">
      <h1 class="w-full my-2 text-5xl font-bold leading-tight text-center text-gray-800">できること</h1>
      <div class="w-full mb-4">
        <div class="h-1 mx-auto gradient w-64 opacity-25 my-0 py-0 rounded-t"></div>
      </div>
      <feature-right headline="カスタマイズ可能な美しい画面" content="あなたがつなげた情報を美しくレイアウトして、あなたの画面にお届けします。">
        <img src="~assets/img/data_trends.svg" alt slot="svg" />
      </feature-right>
      <feature-left headline="いろいろな情報とつながる" content="ソーシャルネットワークからインターネット家電までいろいろな情報とつながります。">
        <img src="~assets/img/connected_world.svg" alt slot="svg" />
      </feature-left>
    </div>
  </section>
</template>

<script>
import FeatureRight from '@/components/FeatureRight'
import FeatureLeft from '@/components/FeatureLeft'

export default {
  name: 'Features',
  components: {
    'feature-right': FeatureRight,
    'feature-left': FeatureLeft
  }
}
</script>
