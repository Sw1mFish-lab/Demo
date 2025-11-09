<template>
	<view class="bar" style="display: flex;">
		<view class="botton" :class="currentMenu === 'home' ? 'currentMenu' : ''" style="flex: 1.7;margin-left: 5px;margin-right: 5px;
					display: flex;justify-content: center;" @click="toHome">
			<view style="display: block;">
				<view style="display: flex;justify-content: center;margin-top: -2px">
					<image src="/icons/Home.png" style="width: 32px;height: 32px;margin-top: 4px;"></image>
				</view>
				<view style="margin-top: -6px;"><text>Home</text></view>
			</view>
		</view>
		<view class="botton" :class="currentMenu === 'device' ? 'currentMenu' : ''" style="flex: 1.7;margin-right: 5px;
								display: flex;justify-content: center;" @click="toDevice">
			<view style="display: block;">
				<view style="display: flex;justify-content: center;margin-top: -2px">
					<image src="/icons/Watch.png" style="width: 32px;height: 32px;margin-top: 4px;"></image>
				</view>
				<view style="margin-top: -6px;"><text>Device</text></view>
			</view>
		</view>
		<view class="botton" style="flex: 3.2;">
			<!-- <view class="add-devices"> -->
			<view class="add-devices" :class="currentMenu === 'scan' ? 'currentMenu' : ''"  @click="toScan">
				<image src="/icons/Camera.png" style="width: 40px;height: 40px;"></image>
			</view>
		</view>

		<view class="botton" :class="currentMenu === 'Plan' ? 'currentMenu' : ''" style="flex: 1.7;margin-left: 5px;margin-right: 5px;
							display: flex;justify-content: center;" @click="toPlan">
			<view style="display: block;">
				<view style="display: flex;justify-content: center;margin-top: -2px">
					<image src="/icons/Archive.png" style="width: 32px;height: 32px;margin-top: 4px;"></image>
				</view>
				<view style="margin-top: -6px;"><text>Plan</text></view>
			</view>
		</view>
		<view class="botton" :class="currentMenu === 'profile' ? 'currentMenu' : ''" style="flex: 1.7;margin-right: 5px;
							display: flex;justify-content: center;" @click="toProfile">
			<view style="display: block;">
				<view style="display: flex;justify-content: center;margin-top: -2px">
					<image src="/icons/User1.png" style="width: 32px;height: 32px;margin-top: 4px;"></image>
				</view>
				<view style="margin-top: -6px;"><text>Profile</text></view>
			</view>
		</view>
	</view>
</template>

<script setup>	
	import { ref, watch } from 'vue';
	
	const props = defineProps({
		currentMenu: 'home'
	})
	
	
	function toHome() {
		props.currentMenu = 'home'
		uni.reLaunch({
			url: '/pages/index/index'
		})
	}
	function toPlan() {
		props.currentMenu = 'plan'
		uni.reLaunch({
			url: '/pages/Plan/Plan'
		})
	}
	function toDevice() {
			props.currentMenu = 'device'
			uni.reLaunch({
				url: '/pages/device/device'
			})
		}
		function toProfile() {
				props.currentMenu = 'profile'
				uni.reLaunch({
					url: '/pages/profile/profile'
				})
			}
		function toScan() {
				props.currentMenu = 'Scan'
				uni.reLaunch({
					url: '/pages/scan/scan'
				})
			}
</script>

<style>
	.currentMenu {
		background-color: rgb(255, 255, 255);
		box-shadow: 0 6rpx 15rpx darkgray;
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