<script setup lang="ts">
import { getHomeGoodsGuessLikeAPI } from '@/services/home'
import type { PageParams } from '@/types/global'
import type { GuessItem } from '@/types/home'
import { onMounted, ref } from 'vue'

//分页参数
const pageParams: Required<PageParams> = {
  page: 1,
  pageSize: 10,
}
//猜你喜欢的列表
const guessList = ref<GuessItem[]>([])
// 已结束标记
const finish = ref(false)
//获取猜你喜欢数据
const getHomeGoodsGuessLikeData = async () => {
  // 退出判断
  if (finish.value === true) {
    return uni.showToast({ icon: 'none', title: '没有更多数据了' })
  }
  const res = await getHomeGoodsGuessLikeAPI(pageParams)
  // guessList.value = res.result.items
  //数组的追加
  guessList.value.push(...res.result.items)
  //分页的条件
  if (pageParams.page < res.result.pages) {
    //页码的累加
    pageParams.page++
  } else {
    finish.value = true
  }
}

//重置数据
const resetData = () => {
  pageParams.page = 1
  guessList.value = []
  finish.value = false
}
//组件挂载完毕
onMounted(() => {
  getHomeGoodsGuessLikeData()
})

//暴露方法
defineExpose({
  getMore: getHomeGoodsGuessLikeData,
  resetData,
})
</script>

<template>
  <!-- 猜你喜欢 -->
  <view class="caption">
    <text class="text">猜你喜欢</text>
  </view>
  <view class="guess">
    <navigator
      class="guess-item"
      v-for="item in guessList"
      :key="item.id"
      :url="`/pages/goods/goods?id=${item.id}`"
    >
      <image class="image" mode="aspectFill" :src="item.picture"></image>
      <view class="name">{{ item.name }}</view>
      <view class="price">
        <text class="small">¥</text>
        <text>{{ item.price }}</text>
      </view>
    </navigator>
  </view>
  <view class="loading-text">{{ finish ? '没有更多数据~' : '正在加载...' }}</view>
</template>

<style lang="scss">
@import '@/components/styles/XtxGuess.scss';
</style>
