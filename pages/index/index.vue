<template>
	<view class="content">
		<!-- <image mode="widthFix" style="width: 100%;" src="/static/eweim.jpg"></image> -->
	</view>
</template>

<script>
	export default {
		data() {
			return {
				url: ""
			}
		},
		// http://localhost:8080?a=qwimg1
		// / http://localhost:8080?a=yeji
		onLoad() {
			uni.showLoading({
				title: "加载中"
			})
			var config = ['https://frdzhtsignup.zsyflive.com/?exType=4&exhId=123',
				'https://frdzhtsignup.zsyflive.com/?exType=9&exhId=129',
				'https://frdzhtsignup.zsyflive.com/?exType=8&exhId=137',
			];
			var url = window.location.href;


			if (url.indexOf("/2025/lyqw") >= 0) { //临沂全屋
				console.log("临沂全屋",url);
				window.location.href = "https://frdzhtsignup.zsyflive.com/frd/uPV0XyoMn4LUvuBA3RyK3RimxLoei7fwN0mnI76pqRs=";
				uni.hideLoading();
			}else if (url.indexOf("/2025/xawj") >= 0) { //西安五金
				window.location.href = "https://frdzhtsignup.zsyflive.com/frd/geZ9NPEkkaKdmmmIwn2T9L1IFA+eUgovWK+K240qeOw=";
				uni.hideLoading();
			}else if (url.indexOf("/2025/hbwh") >= 0) { //湖北武汉
				window.location.href = "https://frdzhtsignup.zsyflive.com/frd/hxyHo131uBAFMR@hgnHIQSPzYiMZs3MFCBKXjxrw6kE=";
				uni.hideLoading();
			}  
			// else if (url.indexOf("/2024/jbh") >= 0) { //建博会
			// 	window.location.href =
			// 	"https://frdzhtsignup.zsyflive.com/frd/sNXpjJYxu9NpsWjvr2s7P93mog5m81CknbMp3LUR5n0=";
			// 	uni.hideLoading();
			// } else if (url.indexOf("/2024/gxmyz") >= 0) { //广西木业展
			// 	window.location.href =
			// 	"https://frdzhtsignup.zsyflive.com/frd/h2dYlPXb4+cQZzrtxCYZdvGRnvweA1Rvv8emKZd+yNA=";
			// 	uni.hideLoading();
			// } else if (url.indexOf("/2024/xawjz") >= 0) { //西安五金展
			// 	window.location.href =
			// 	"https://frdzhtsignup.zsyflive.com/frd/geZ9NPEkkaKdmmmIwn2T9Injv+M1pr969uxwjqjIcUU=";
			// 	uni.hideLoading();
			// } else if (url.indexOf("/2024/qjh") >= 0) { //秋交会
			// 	window.location.href =
			// 	"https://frdzhtsignup.zsyflive.com/frd/9QU+TdjAVRmbrjHzKHbsSrFQK05KV@iE+xC0qhxNzIk=";
			// 	uni.hideLoading();
			// } else if (url.indexOf("/2024/ljh") >= 0) { //林交会
			// 	window.location.href =
			// 	"https://frdzhtsignup.zsyflive.com/frd/QFyZC5QyO+JcdEPIRcOhLMyVLYVYE4BaTTLeaCgBtLo=";
			// 	uni.hideLoading();
			// } else if (url.indexOf("/2024/lbh") >= 0) { //绿博会
			// 	window.location.href =
			// 	"https://frdzhtsignup.zsyflive.com/frd/scOC6RLbHDbEfwIAP0zN+7IliKoX@IXGl7WbT5BAGK4=";
			// 	uni.hideLoading();
			// } else if (url.indexOf("/2024/tbh") >= 0) { //体博会
			// 	window.location.href =
			// 	"https://frdzhtsignup.zsyflive.com/frd/Vfth@Oze6IYvM4vX3yRHfh0m30VCZn8c9IUj3bShqdE=";
			// 	uni.hideLoading();
			// } else if (url.indexOf("/2024/whdzjj") >= 0) { //武汉定制家居
			// 	window.location.href =
			// 	"https://frdzhtsignup.zsyflive.com/frd/hxyHo131uBAFMR@hgnHIQajdP1cIbROkeJE3+Rnz0jU=";
			// 	uni.hideLoading();
			// } else if (url.indexOf("qwimg1") >= 0) { //林交会
			// 	uni.reLaunch({
			// 		url: "/pages/qwimg1/qwimg1"
			// 	})
			// } else if (url.indexOf("qwvideo1") >= 0) { //林交会
			// 	uni.reLaunch({
			// 		url: "/pages/qw_video1/qw_video1"
			// 	})
			// } else if (url.indexOf("chenxunwang") >= 0) { //林交会
			// 	uni.reLaunch({
			// 		url: "/pages/xuanchuan/xuanchuan"
			// 	})
			// } else if (url.indexOf("zxwlinjh") >= 0) { //林交会
			// 	console.log("启动tiaozhuan 林交会", )
			// 	uni.reLaunch({
			// 		url: "/pages/ljh_zxw/ljh_zxw"
			// 	})
			// } else if (url.indexOf("yejiimg") >= 0) { //林交会
			// 	uni.navigateTo({
			// 		url: "/pages/yejiimg/yejiimg"
			// 	})
			// } else if (url.indexOf("muyetong") >= 0) { //林交会
			// 	window.location.href = "https://muyetong.mianshijing.top";
			// 	uni.hideLoading();
			// } 
			else {
				this.url = url;
				console.log("跳转", url);
				window.location.href = config[2];
				uni.hideLoading();
			}
			setTimeout(res => {
				uni.hideLoading()
			}, 1000)
		},
		methods: {

		}
	}
</script>

<style>
	.content {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}

	.logo {
		height: 200rpx;
		width: 200rpx;
		margin-top: 200rpx;
		margin-left: auto;
		margin-right: auto;
		margin-bottom: 50rpx;
	}

	.text-area {
		display: flex;
		justify-content: center;
	}

	.title {
		font-size: 36rpx;
		color: #8f8f94;
	}
</style>