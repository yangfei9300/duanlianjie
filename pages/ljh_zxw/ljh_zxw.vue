<template>
	<view>
		
		<!-- 林交会展讯网宣传页 -->
		<image src="https://meili-media.oss-cn-beijing.aliyuncs.com/zhanweitu/xiangcun/19a45f933c08315dce6f69779858616.jpg"
		style="width:750rpx" mode="widthFix"
		></image>
		<view class="btn" @click="tourl">前往登记</view>
		
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			tourl(){
				window.location.href="https://frdzhtsignup.zsyflive.com?upUid=13512122686&exhId=129&exType=9";
			},
		}
	}
</script>

<style>
.btn{
	width: 700rpx;
	height: 90rpx;
	background-color:      #279A3F;
	position: fixed;
	bottom: 50rpx;
	left: 25rpx;
	text-align: center;
	line-height: 90rpx;
	border-radius: 10rpx;
	border: 1px solid white;
}
</style>
