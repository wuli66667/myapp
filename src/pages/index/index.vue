<template>
  <view class="container">
    <!--搜索  -->
    <view class="search">
      <!-- 输入框 -->
      <view class="input-box">
        <input type="text" name id />
      </view>
      <!-- 搜索结果 -->
      <view class="content"></view>
    </view>

    <!-- 轮播图 -->
	<swiper class="slide" indicator-dots indicator-color="rgba(255,255,255,.6)" indicator-active-color="#fff" autoplay interval="2000" circular>
		<swiper-item>
			<navigator url="">
				<image src="/static/uploads/banner1.png"></image>
			</navigator>
		</swiper-item>

		<swiper-item>
			<navigator url="">
				<image src="/static/uploads/banner2.png"></image>
			</navigator>
		</swiper-item>

		<swiper-item>
			<navigator url="">
				<image src="/static/uploads/banner3.png"></image>
			</navigator>
		</swiper-item>

	</swiper>
    <!-- 主导航 -->
	<view class="navs">
		<navigator url="">
			<image src="/static/uploads/icon_index_nav_4@2x.png"></image>
		</navigator>

		<navigator url="">
			<image src="/static/uploads/icon_index_nav_3@2x.png"></image>
		</navigator>
		
		<navigator url="">
			<image src="/static/uploads/icon_index_nav_2@2x.png"></image>
		</navigator>
		<navigator url="">
			<image src="/static/uploads/icon_index_nav_1@2x.png"></image>
		</navigator>
	</view>
	 <!-- 时尚女装 -->
	<view class="floors">
		<!-- 一广告 -->
	 	<view class="floor">
		 	<view class ="title">
         		 <image src="http://static.botue.com/ugo/uploads/pic_floor03_title.png"></image>
        	</view>
		</view>
	</view>
  </view>
</template>

<script>
export default {
  data() {
    return {
      title: 'Hello'
    }
  },
  onLoad() {},
  methods: {}
}
</script>

<style lang="less">
.search {
  .input-box {
    padding: 20rpx;
    background-color: #ea4451;
    input {
      height: 60rpx;
      background-color: #fff;
      border-radius: 5rpx;
    }
  }
}
// 轮播图
swiper{
	height: 340rpx;
	image{
		width: 750rpx;
		height: 340rpx;
	}
}
// 主导航
.navs{
	display: flex;
	justify-content: space-between;
	padding: 30rpx 0;
	// background-color: pink;
	navigator{
		width: 128rpx;
		height: 140rpx;
	}

}
// 时尚女装
.floors{
	.title{
		width: 750rpx;
		height: 60rpx;
		padding: 20rpx 0 0 10rpx;
		background-color: #f4f4f4;
	}
}

</style>
