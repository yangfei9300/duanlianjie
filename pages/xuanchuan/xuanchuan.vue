<template>
	<view>
		
		<!-- 秋交会展讯网宣传页 -->
		<image src="https://meili-media.oss-cn-beijing.aliyuncs.com/zhanweitu/xiangcun/f22bdf239c2437fe9164d6786a9b58b.jpg"
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
				window.location.href="https://frdzhtsignup.zsyflive.com?upUid=13512122686&exhId=123&exType=4";
			},
		}
	}
</script>

<style>
.btn{
	width: 700rpx;
	height: 90rpx;
	background-color:     #0080CB;
	position: fixed;
	bottom: 50rpx;
	left: 25rpx;
	text-align: center;
	line-height: 90rpx;
	border-radius: 10rpx;
	border: 1px solid white;
}
</style>
