<template name="skeleton">
  <view class="sk-container">
    <view class="viewport viewport">
      <!-- <view class="tabs tabs">
        <text class="item sk-transparent sk-text-26-6667-935 sk-text" style="background-position-x: 50%;">全部</text>
        <text class="item sk-transparent sk-text-26-6667-783 sk-text" style="background-position-x: 50%;">待付款</text>
        <text class="item sk-transparent sk-text-26-6667-628 sk-text" style="background-position-x: 50%;">待发货</text>
        <text class="item sk-transparent sk-text-26-6667-194 sk-text" style="background-position-x: 50%;">待收货</text>
        <text class="item sk-transparent sk-text-26-6667-655 sk-text" style="background-position-x: 50%;">待评价</text>
        <view class="cursor cursor" style="left:0%"></view>
      </view> -->
      <swiper class="swiper swiper" current="0" autoplay="false">
        <swiper-item
          style="
            position: absolute;
            width: 100%;
            height: 100%;
            transform: translate(0%, 0px) translateZ(0px);
          "
        >
          <view is="pagesOrder/list/components/OrderList">
            <scroll-view scroll-y="true" class="orders OrderList--orders" enable-back-to-top="true">
              <view class="card OrderList--card">
                <view class="status OrderList--status">
                  <text class="date OrderList--date sk-transparent sk-text-14-2857-893 sk-text"
                    >2024-08-17 20:58:45</text
                  >
                  <text class="sk-transparent sk-text-14-2857-610 sk-text">待评价</text>
                  <text
                    class="icon-delete OrderList--icon-delete sk-pseudo sk-pseudo-circle"
                  ></text>
                </view>
                <navigator class="goods OrderList--goods" hover-class="none">
                  <view class="cover OrderList--cover">
                    <image mode="aspectFit" class="sk-image"></image>
                  </view>
                  <view class="meta OrderList--meta">
                    <view
                      class="name OrderList--name ellipsis OrderList--ellipsis sk-transparent sk-text-14-2857-120 sk-text"
                    >
                      七夕礼物·挺拔身姿，隐形内穿矫姿带</view
                    >
                    <view class="type OrderList--type sk-transparent sk-text-22-2222-563 sk-text"
                      >L</view
                    >
                  </view>
                </navigator>
                <view class="payment OrderList--payment">
                  <text
                    class="quantity OrderList--quantity sk-transparent sk-text-0-0000-647 sk-text"
                    style="background-position-x: 100%"
                    >共1件商品</text
                  >
                  <text
                    class="sk-transparent sk-text-0-0000-320 sk-text"
                    style="background-position-x: 100%"
                    >实付</text
                  >
                  <text class="amount OrderList--amount sk-transparent"
                    ><text class="symbol OrderList--symbol sk-transparent sk-opacity">¥</text
                    >154</text
                  >
                </view>
                <view class="action OrderList--action">
                  <navigator
                    class="button OrderList--button secondary OrderList--secondary sk-transparent sk-text-14-2857-525 sk-text"
                    hover-class="none"
                  >
                    再次购买
                  </navigator>
                </view>
              </view>
              <view class="card OrderList--card">
                <view class="status OrderList--status">
                  <text class="date OrderList--date sk-transparent sk-text-14-2857-91 sk-text"
                    >2024-08-17 16:13:11</text
                  >
                  <text class="sk-transparent sk-text-14-2857-605 sk-text">待发货</text>
                </view>
                <navigator class="goods OrderList--goods" hover-class="none">
                  <view class="cover OrderList--cover">
                    <image mode="aspectFit" class="sk-image"></image>
                  </view>
                  <view class="meta OrderList--meta">
                    <view
                      class="name OrderList--name ellipsis OrderList--ellipsis sk-transparent sk-text-14-2857-711 sk-text"
                    >
                      钻石陶瓷涂层多用锅18cm 小奶锅</view
                    >
                    <view class="type OrderList--type sk-transparent sk-text-22-2222-929 sk-text"
                      >黑色， 中国， 20cm</view
                    >
                  </view>
                </navigator>
                <view class="payment OrderList--payment">
                  <text
                    class="quantity OrderList--quantity sk-transparent sk-text-0-0000-486 sk-text"
                    style="background-position-x: 100%"
                    >共1件商品</text
                  >
                  <text
                    class="sk-transparent sk-text-0-0000-845 sk-text"
                    style="background-position-x: 100%"
                    >实付</text
                  >
                  <text class="amount OrderList--amount sk-transparent"
                    ><text class="symbol OrderList--symbol sk-transparent sk-opacity">¥</text
                    >128</text
                  >
                </view>
                <view class="action OrderList--action">
                  <navigator
                    class="button OrderList--button secondary OrderList--secondary sk-transparent sk-text-14-2857-507 sk-text"
                    hover-class="none"
                  >
                    再次购买
                  </navigator>
                </view>
              </view>
              <view class="card OrderList--card">
                <view class="status OrderList--status">
                  <text class="date OrderList--date sk-transparent sk-text-14-2857-353 sk-text"
                    >2024-08-17 14:18:16</text
                  >
                  <text class="sk-transparent sk-text-14-2857-125 sk-text">待评价</text>
                  <text
                    class="icon-delete OrderList--icon-delete sk-pseudo sk-pseudo-circle"
                  ></text>
                </view>
                <navigator class="goods OrderList--goods" hover-class="none">
                  <view class="cover OrderList--cover">
                    <image mode="aspectFit" class="sk-image"></image>
                  </view>
                  <view class="meta OrderList--meta">
                    <view
                      class="name OrderList--name ellipsis OrderList--ellipsis sk-transparent sk-text-14-2857-51 sk-text"
                    >
                      钻石陶瓷涂层多用锅18cm 小奶锅</view
                    >
                    <view class="type OrderList--type sk-transparent sk-text-22-2222-389 sk-text"
                      >蓝色， 中国， 30cm</view
                    >
                  </view>
                </navigator>
                <view class="payment OrderList--payment">
                  <text
                    class="quantity OrderList--quantity sk-transparent sk-text-0-0000-553 sk-text"
                    style="background-position-x: 100%"
                    >共1件商品</text
                  >
                  <text
                    class="sk-transparent sk-text-0-0000-700 sk-text"
                    style="background-position-x: 100%"
                    >实付</text
                  >
                  <text class="amount OrderList--amount sk-transparent"
                    ><text class="symbol OrderList--symbol sk-transparent sk-opacity">¥</text
                    >128</text
                  >
                </view>
                <view class="action OrderList--action">
                  <navigator
                    class="button OrderList--button secondary OrderList--secondary sk-transparent sk-text-14-2857-611 sk-text"
                    hover-class="none"
                  >
                    再次购买
                  </navigator>
                </view>
              </view>
            </scroll-view>
          </view>
        </swiper-item>
      </swiper>
    </view>
  </view>
</template>

<style>
.sk-transparent {
  color: transparent !important;
}

.sk-text-26-6667-935 {
  background-image: linear-gradient(
    transparent 26.6667%,
    #eeeeee 0%,
    #eeeeee 73.3333%,
    transparent 0%
  ) !important;
  background-size: 100% 60rpx;
  position: relative !important;
}

.sk-text {
  background-origin: content-box !important;
  background-clip: content-box !important;
  background-color: transparent !important;
  color: transparent !important;
  background-repeat: repeat-y !important;
}

.sk-text-26-6667-783 {
  background-image: linear-gradient(
    transparent 26.6667%,
    #eeeeee 0%,
    #eeeeee 73.3333%,
    transparent 0%
  ) !important;
  background-size: 100% 60rpx;
  position: relative !important;
}

.sk-text-26-6667-628 {
  background-image: linear-gradient(
    transparent 26.6667%,
    #eeeeee 0%,
    #eeeeee 73.3333%,
    transparent 0%
  ) !important;
  background-size: 100% 60rpx;
  position: relative !important;
}

.sk-text-26-6667-194 {
  background-image: linear-gradient(
    transparent 26.6667%,
    #eeeeee 0%,
    #eeeeee 73.3333%,
    transparent 0%
  ) !important;
  background-size: 100% 60rpx;
  position: relative !important;
}

.sk-text-26-6667-655 {
  background-image: linear-gradient(
    transparent 26.6667%,
    #eeeeee 0%,
    #eeeeee 73.3333%,
    transparent 0%
  ) !important;
  background-size: 100% 60rpx;
  position: relative !important;
}

.sk-text-14-2857-893 {
  background-image: linear-gradient(
    transparent 14.2857%,
    #eeeeee 0%,
    #eeeeee 85.7143%,
    transparent 0%
  ) !important;
  background-size: 100% 39.2rpx;
  position: relative !important;
}

.sk-text-14-2857-610 {
  background-image: linear-gradient(
    transparent 14.2857%,
    #eeeeee 0%,
    #eeeeee 85.7143%,
    transparent 0%
  ) !important;
  background-size: 100% 39.2rpx;
  position: relative !important;
}

.sk-text-14-2857-120 {
  background-image: linear-gradient(
    transparent 14.2857%,
    #eeeeee 0%,
    #eeeeee 85.7143%,
    transparent 0%
  ) !important;
  background-size: 100% 36.4rpx;
  position: relative !important;
}

.sk-text-22-2222-563 {
  background-image: linear-gradient(
    transparent 22.2222%,
    #eeeeee 0%,
    #eeeeee 77.7778%,
    transparent 0%
  ) !important;
  background-size: 100% 43.2rpx;
  position: relative !important;
}

.sk-text-0-0000-647 {
  background-image: linear-gradient(
    transparent 0%,
    #eeeeee 0%,
    #eeeeee 100%,
    transparent 0%
  ) !important;
  background-size: 100% 24rpx;
  position: relative !important;
}

.sk-text-0-0000-320 {
  background-image: linear-gradient(
    transparent 0%,
    #eeeeee 0%,
    #eeeeee 100%,
    transparent 0%
  ) !important;
  background-size: 100% 28rpx;
  position: relative !important;
}

.sk-opacity {
  opacity: 0 !important;
}

.sk-text-14-2857-525 {
  background-image: linear-gradient(
    transparent 14.2857%,
    #eeeeee 0%,
    #eeeeee 85.7143%,
    transparent 0%
  ) !important;
  background-size: 100% 36.4rpx;
  position: relative !important;
}

.sk-text-14-2857-91 {
  background-image: linear-gradient(
    transparent 14.2857%,
    #eeeeee 0%,
    #eeeeee 85.7143%,
    transparent 0%
  ) !important;
  background-size: 100% 39.2rpx;
  position: relative !important;
}

.sk-text-14-2857-605 {
  background-image: linear-gradient(
    transparent 14.2857%,
    #eeeeee 0%,
    #eeeeee 85.7143%,
    transparent 0%
  ) !important;
  background-size: 100% 39.2rpx;
  position: relative !important;
}

.sk-text-14-2857-711 {
  background-image: linear-gradient(
    transparent 14.2857%,
    #eeeeee 0%,
    #eeeeee 85.7143%,
    transparent 0%
  ) !important;
  background-size: 100% 36.4rpx;
  position: relative !important;
}

.sk-text-22-2222-929 {
  background-image: linear-gradient(
    transparent 22.2222%,
    #eeeeee 0%,
    #eeeeee 77.7778%,
    transparent 0%
  ) !important;
  background-size: 100% 43.2rpx;
  position: relative !important;
}

.sk-text-0-0000-486 {
  background-image: linear-gradient(
    transparent 0%,
    #eeeeee 0%,
    #eeeeee 100%,
    transparent 0%
  ) !important;
  background-size: 100% 24rpx;
  position: relative !important;
}

.sk-text-0-0000-845 {
  background-image: linear-gradient(
    transparent 0%,
    #eeeeee 0%,
    #eeeeee 100%,
    transparent 0%
  ) !important;
  background-size: 100% 28rpx;
  position: relative !important;
}

.sk-text-14-2857-507 {
  background-image: linear-gradient(
    transparent 14.2857%,
    #eeeeee 0%,
    #eeeeee 85.7143%,
    transparent 0%
  ) !important;
  background-size: 100% 36.4rpx;
  position: relative !important;
}

.sk-text-14-2857-353 {
  background-image: linear-gradient(
    transparent 14.2857%,
    #eeeeee 0%,
    #eeeeee 85.7143%,
    transparent 0%
  ) !important;
  background-size: 100% 39.2rpx;
  position: relative !important;
}

.sk-text-14-2857-125 {
  background-image: linear-gradient(
    transparent 14.2857%,
    #eeeeee 0%,
    #eeeeee 85.7143%,
    transparent 0%
  ) !important;
  background-size: 100% 39.2rpx;
  position: relative !important;
}

.sk-text-14-2857-51 {
  background-image: linear-gradient(
    transparent 14.2857%,
    #eeeeee 0%,
    #eeeeee 85.7143%,
    transparent 0%
  ) !important;
  background-size: 100% 36.4rpx;
  position: relative !important;
}

.sk-text-22-2222-389 {
  background-image: linear-gradient(
    transparent 22.2222%,
    #eeeeee 0%,
    #eeeeee 77.7778%,
    transparent 0%
  ) !important;
  background-size: 100% 43.2rpx;
  position: relative !important;
}

.sk-text-0-0000-553 {
  background-image: linear-gradient(
    transparent 0%,
    #eeeeee 0%,
    #eeeeee 100%,
    transparent 0%
  ) !important;
  background-size: 100% 24rpx;
  position: relative !important;
}

.sk-text-0-0000-700 {
  background-image: linear-gradient(
    transparent 0%,
    #eeeeee 0%,
    #eeeeee 100%,
    transparent 0%
  ) !important;
  background-size: 100% 28rpx;
  position: relative !important;
}

.sk-text-14-2857-611 {
  background-image: linear-gradient(
    transparent 14.2857%,
    #eeeeee 0%,
    #eeeeee 85.7143%,
    transparent 0%
  ) !important;
  background-size: 100% 36.4rpx;
  position: relative !important;
}

.sk-image {
  background: #efefef !important;
}

.sk-pseudo::before,
.sk-pseudo::after {
  background: #efefef !important;
  background-image: none !important;
  color: transparent !important;
  border-color: transparent !important;
}

.sk-pseudo-rect::before,
.sk-pseudo-rect::after {
  border-radius: 0 !important;
}

.sk-pseudo-circle::before,
.sk-pseudo-circle::after {
  border-radius: 50% !important;
}

.sk-container {
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  overflow: hidden;
  background-color: transparent;
}
</style>
