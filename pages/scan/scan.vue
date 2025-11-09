<template>
	<view>
		<customTabbarVue current-menu="scan" style="position: fixed;z-index: 1000;"></customTabbarVue>
	</view>
	<view class="scan">
		<view class="scan-camera" style="margin-left: auto;margin-right: auto;margin-top: 300rpx;">
			
		</view>
		<view style="width: 70px;height: 70px;background-color: white;display: flex;flex-direction: column;margin-top: 100rpx;margin-left: auto;margin-right: auto;border-radius: 9px;">
			<image src="/icons/Camera.png" style="width: 50px;height: 50px;margin-left: auto;margin-right: auto;margin-top: 10px"></image>
		</view>
	</view>
</template>

<script setup>
	import customTabbarVue from '@/components/customTabbar/customTabbar.vue';
</script>

<style>
	.scan{
		height: 100%;
		width: 100%;
		background-color: #d9d9d9;
	}
	.scan-camera{
		height: 387px;
		width: 387px;
		background-color: black;
	}
</style>
