
<template>
	<customTabbarVue current-menu="device"></customTabbarVue>
	<view class="container">
		<view style="margin-left: 3px;"><text style="font-size: 36px;">Devices</text></view>
		<view class="Device-card" style="display: flex;">
			<view style="flex: 5;">
				<view class="watch-name">watch 4e</view>
				<view style="margin-top: 13px;margin-left: 27px;display: flex;">
					<image src="/icons/Battery.png" style="width: 26px;height: 16px;"></image>
					<view style="margin-top: -5px;"><text style="margin-left: 8px;">100%</text></view>
				</view>
				<view style="margin-top: 8px;display: flex;margin-left: 29px;">
					<image src="/icons/Bluetooth.png" style="width: 20px;height: 20px;"></image>
					<view style="margin-top: -4px;margin-left: 14px;"><text>Connected</text></view>
				</view>
				<view class="botton1" style="text-align: center;line-height:43px"><text style="color: white;font-size: 16px;">Details</text></view>
			</view>
			<view style="flex: 5;">
				<image src="/icons/Watch4E.png" style="width: 194px;height: 194px;"></image>
			</view>
		</view>
		<view style="margin-top: 61px;font-size: 20px;line-height: 32px;">Functions</view>
		<view class="functions" style="display: flex;text-align: center; margin-top: 31px;">
			<view style="flex: 3;">
				<view><image src="/icons/Activity.png" style="width: 48px;height: 48px;"></image></view>
				<view><text>Activity</text></view>
			</view>
			<view style="flex: 3;">
				<view><image src="/icons/Alert triangle.png" style="width: 48px;height: 48px;"></image></view>
				<view><text>S.O.S</text></view>
			</view>
			<view style="flex: 3;">
				<view><image src="/icons/Edit.png" style="width: 48px;height: 48px;"></image></view>
				<view><text>Edit</text></view>
			</view>
		</view>
		<view class="functions" style="display: flex;text-align: center; margin-top: 10px;">
			<view style="flex: 3;">
				<view><image src="/icons/Headphones.png" style="width: 48px;height: 48px;"></image></view>
				<view><text>Music</text></view>
			</view>
			<view style="flex: 3;">
				<view><image src="/icons/Instagram.png" style="width: 48px;height: 48px;"></image></view>
				<view><text>APP</text></view>
			</view>
			<view style="flex: 3;">
				<view><image src="/icons/Mail.png" style="width: 48px;height: 48px;"></image></view>
				<view><text>Mail</text></view>
			</view>
		</view>
	</view>
</template>

<script setup>
	import customTabbarVue from '@/components/customTabbar/customTabbar.vue';
</script>

<style>
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
		padding-left: 13px;
		padding-right: 13px;
		padding-top: 65px;
		box-sizing: border-box;
		background-color: white;
	}
	.Device-card{
		height: 200px;
		width: 100%;
		background-color: #d9d9d9;
		margin-top: 61px;
		border-radius: 8px;
		box-shadow: 0 6rpx 15rpx darkgray;
	}
	.watch-name{
		font-family: BebasNeue-1;
		font-size: 32px;
		line-height: 28px;
		margin-left: 28px;
		margin-top: 28px;
	}
	.botton1{
		width: 81px;
		height: 44px;
		border-radius: 99px;
		background-color: #494949;
		margin-left: 20px;
		margin-top: 22px;
	}
	.functions{
		width: 100%;
		height: 100px;
	}
</style>