<template>
	<view>
		<customTabbarVue current-menu="home"></customTabbarVue>
	</view>
	<view class="container">
		<view class="container-header"><text style="margin-left: 16px;position: fixed;top: 25px;">AllerFree Buddy</text>
		</view>
		<view class="container-search">
			<image src="@/static/logo.png" style="width: 40px;height: 40px;border-radius: 50px;"></image>
			<view class="search-input">
				<image src="/icons/Search.png"
					style="width: 20px;height: 18px;margin-top: 9px;margin-left: 10px;margin-top: 10px;"></image>
				<input style="width: 100%; height: 100%; margin-left: 20rpx;" placeholder="Search"
					placeholder-style="margin-left: 0px;">
			</view>
		</view>
		<view class="Card">Allergen Card</view>
		<view class="HealthCertification">
			<view class="HCText">HEALTH CERTIFICATE</view>
			<view style="display: flex">
				<view style="flex: 6;margin-top: 12px;" class="certification-body">
					<view style="display: flex;">
						<view style="width: 20px;height: 20px;">
							<image src="/icons/Filter.png" style="width: 20px;height: 20px;"></image>
						</view>
						<text style="margin-left: 7px;margin-top: -3px;">Testing Organization</text>
					</view>
					<view style="display: flex;margin-top: 10px;">
						<view style="width: 20px;height: 20px;">
							<image src="/icons/Clock.png" style="width: 20px;height: 20px;"></image>
						</view>
						<text style="margin-left: 7px;margin-top: -3px;">Test Date</text>
					</view>
					<view style="display: flex;margin-top: 10px;">
						<view style="width: 20px;height: 20px;">
							<image src="/icons/Align justify.png" style="width: 20px;height: 20px;"></image>
						</view>
						<text style="margin-left: 7px;margin-top: -3px;">Allergen</text>
					</view>
					<view class="Details" style="text-align: center;line-height: 44px;">
						<text style="color: white;">Details</text>
					</view>
				</view>
				<view style="flex: 4;margin-top: 12px;">
					<view class="userImgContainer">
						<image src="/icons/User.png" class="userImg"></image>
					</view>
				</view>
			</view>
		</view>
		<view style="margin-top: 47px;font-family: noah-regular-2;font-size: 20px;">
			<text>Medical Check-up</text>
		</view>
		<view class="check-up">
			<view style="display: flex;margin-left: 20px;margin-top: 14px;">
				<text>Allergy Test</text>
				<view class="Book" style="text-align: center;line-height:28px"><text
						style="color: white;font-size: 14px;">Book</text></view>
			</view>
			<view style="display: flex;margin-left: 20px;margin-top: 14px;margin-top: 46px;">
				<text>Skin prick test</text>
				<view class="Book" style="text-align: center;line-height:28px"><text
						style="color: white;font-size: 14px;">Book</text></view>
			</view>
			<view style="display: flex;margin-left: 20px;margin-top: 14px;margin-top: 46px;">
				<text>Blood allergy test (IgE test)</text>
				<view class="Book" style="text-align: center;line-height:28px"><text
						style="color: white;font-size: 14px;">Book</text></view>
			</view>
		</view>
	</view>
	<Card></Card>
</template>

<script setup>
	import customTabbarVue from '@/components/customTabbar/customTabbar.vue';
	import Card from '@/components/Card.vue';
	
function toDevice() {
	uni.reLaunch({
		url: '/pages/device/device'
	})
	// 页面栈  底【】顶 《- -》
	// top 10
}

</script>


<style>
	@font-face {
		font-family: "bodytextslim-light-5";
		src: url("@/static/bodytextslim-light-5.otf");
		font-weight: normal;
		font-style: normal;
	}

	@font-face {
		font-family: "noah-regular-2";
		src: url("@/static/noah-regular-2.otf");
		font-weight: normal;
		font-style: normal;
	}

	@font-face {
		font-family: "BebasNeue-1";
		src: url("@/static/BebasNeue-1.otf");
		font-weight: normal;
		font-style: normal;
	}

	.container {
		width: 100%;
		height: 100%;
		margin: 0;
		padding: 0;
		padding-left: 16px;
		padding-right: 16px;
		padding-top: 40px;
		box-sizing: border-box;
		background-color: white;
	}

	.container .container-header {
		font-family: "noah-regular-2";
		transform: scaleX(1.2);
		transform-origin: left;
		disp: flex;
		background-color: white;
		line-height: 28px;
		font-size: 32px;
		position: fixed;
		z-index: 1000;
		width: 100%;
		margin-top: -40px;
		height: 65px;
		left: 0px;
	}

	.container-search {
		display: flex;
		background-color: white;
		width: 100%;
		height: 40px;
		margin-top: 80rpx;
	}

	.search-input {
		display: flex;
		margin-left: 8px;
		margin-top: 2px;
		margin-bottom: 2px;
		flex: 1;
		height: 36px;
		background-color: #D9D9D9;
		border-radius: 8px;
		box-shadow: 0 6rpx 15rpx darkgray;
	}

	.Card {
		font-family: "noah-regular-2";
		font-size: 20px;
		margin-top: 24px;
	}

	.HealthCertification {
		display: flex;
		flex-direction: column;
		margin-top: 24px;
		background-color: #EEECEC;
		width: 100%;
		height: 192px;
		border-radius: 8px;
		box-shadow: 0 6rpx 15rpx darkgray;
	}

	.HCText {
		font-family: "BebasNeue-1";
		width: 100%;
		font-size: 32px;
		line-height: 16px;
		margin-top: 18px;
		margin-left: 14px;
	}

	.certification-body {
		width: 100%;
		height: 100%;
		margin-left: 14px;
	}

	.Details {
		height: 44px;
		width: 84px;
		background-color: #494949;
		border-radius: 8px;
		box-shadow: 0 6rpx 15rpx darkgray;
		margin-top: 11px;
	}

	.userImgContainer {
		width: 127px;
		height: 127px;
		background-image: url("@/icons/Square.png");
		background-size: 100%;
		/* 子元素水平垂直居中 */
		display: flex;
		justify-content: center;
		align-items: center;
	}

	.userImg {
		width: 95px;
		height: 95px;
	}

	.check-up {
		margin-top: 24px;
		height: 228px;
		width: 100%;
		background-color: #F4F0EB;
		border-radius: 8px;
		box-shadow: 0 6rpx 15rpx darkgray;
		font-size: 20px;
		display: flex;
		flex-direction: column;
	}

	.Book {
		height: 32px;
		width: 65px;
		background-color: #212121;
		border-radius: 20px;
		margin-left: auto;
		margin-right: 14px;

	}

	.bar {
		height: 61px;
		background-color: #f0f0f0f0;
		margin-top: auto;
		position: fixed;
		bottom: 5px;
		left: 3px;
		right: 3px;
		border-radius: 8px;
		box-shadow: 0 7rpx 15rpx darkgray;
	}

	.botton {
		background-color: #f0f0f0f0;
		height: 50px;
		width: 50px;
		margin-top: 5.5px;
		border-radius: 8px;
	}

	.add-devices {
		width: 70px;
		height: 70px;
		background-color: #f4f0eb;
		border-radius: 999px;
		margin-left: auto;
		margin-right: auto;
		box-shadow: 0 7rpx 15rpx darkgray;
		margin-top: -23px;
		display: flex;
		justify-content: center;
		align-items: center;
	}
</style>