<template>
	<view>
		<customTabbarVue current-menu="profile" style="position: fixed;z-index: 1000;"></customTabbarVue>
	</view>
	<view class="profile-page">
		<view style="display: flex;">
			<view style="width:500px;height: 500px;background-color: #D4AEAE;border-radius: 999px;margin-top: -200px;margin-left: -200px;">
				<view style="width:300px;height: 300px;background-color: #BDEBFF;border-radius: 999px;margin-left: 450px;margin-top: 70px;"></view>
			</view>
			<view style="width: 120px;height: 120px;display: flex;">
				<image src="/icons/UserPhoto.png" style="width: 120px;height: 120px;margin-left: -280px;margin-top: 100px;"></image>
				<view style="font-size: 40px;margin-top: 130px;margin-left: 30px;">UserName</view>
			</view>
		</view>
		<view style="background-color: white;width: 100%;height: 100%;border-radius: 30px;margin-top: -50px;position: absolute;z-index: 999;">
			<view style="display: flex;height: 100px;margin-top: 43px;width: 100%;">
				<view style="display: flex;align-items:center;justify-content: center; 1;width: 100px;height: 100px;background-color: #f0f0f0;margin-left: 19px;margin-right: 19px;border-radius: 9px;box-shadow: 0 6rpx 15rpx darkgray;">
					<view style="display: block;display: flex;align-items:center;justify-content: center;flex-direction: column;gap: 8px;">
						<image src="/icons/Server.png" style="width: 32px;height: 32px;"></image>
						<view style="width: 100%;">Service</view>
					</view>
				</view>
				<view style="display: flex;align-items:center;justify-content: center; 1;width: 100px;height: 100px;background-color: #f0f0f0;margin-left: auto;margin-right: auto;border-radius: 9px;box-shadow: 0 6rpx 15rpx darkgray;">
									<view style="display: block;display: flex;align-items:center;justify-content: center;flex-direction: column;gap: 8px;">
										<image src="/icons/Book.png" style="width: 32px;height: 32px;"></image>
										<view style="width: 100%;">Dietary Palns</view>
									</view>
								</view>
				<view style="display: flex;align-items:center;justify-content: center; 1;width: 100px;height: 100px;background-color: #f0f0f0;margin-left: 19px;margin-right: 19px;border-radius: 9px;box-shadow: 0 6rpx 15rpx darkgray;">
									<view style="display: block;display: flex;align-items:center;justify-content: center;flex-direction: column;gap: 8px;">
										<image src="/icons/gmail_groups.png" style="width: 32px;height: 32px;"></image>
										<view style="width: 100%;">Friends</view>
									</view>
								</view>
			</view>
			<view style="display: flex;height: 100px;width:auto;margin-top: 43px;">
				<view style="display: flex;align-items:center;justify-content: center; 1;width: 100px;height: 100px;background-color: #f0f0f0;margin-left: 19px;margin-right: 19px;border-radius: 9px;box-shadow: 0 6rpx 15rpx darkgray;">
									<view style="display: block;display: flex;align-items:center;justify-content: center;flex-direction: column;gap: 8px;">
										<image src="/icons/favorite.png" style="width: 32px;height: 32px;"></image>
										<view style="width: 100%;">Favorites</view>
									</view>
								</view>
				<view style="display: flex;align-items:center;justify-content: center; 1;width: 100px;height: 100px;background-color: #f0f0f0;margin-left: auto;margin-right: auto;border-radius: 9px;box-shadow: 0 6rpx 15rpx darkgray;">
									<view style="display: block;display: flex;align-items:center;justify-content: center;flex-direction: column;gap: 8px;">
										<image src="/icons/Edit 2.png" style="width: 32px;height: 32px;"></image>
										<view style="width: 100%;">Notes</view>
									</view>
								</view>
				<view style="display: flex;align-items:center;justify-content: center; 1;width: 100px;height: 100px;background-color: #f0f0f0;margin-left: 19px;margin-right: 19px;border-radius: 9px;box-shadow: 0 6rpx 15rpx darkgray;">
									<view style="display: block;display: flex;align-items:center;justify-content: center;flex-direction: column;gap: 8px;">
										<image src="/icons/Credit card.png" style="width: 32px;height: 32px;"></image>
										<view style="width: 100%;">Balance</view>
									</view>
								</view>
			</view>
			<view class="more-functions">
				<view style="display: block;width: 100%;">
					<view class="functioncard" style="display: flex;">
						<image src="/icons/settings.png" style="width: 30px;height: 30px;margin-top: 10px;margin-left: 12px;"></image>
						<view style="line-height: 45x;margin-left: 30px;margin-top: 12px;">Setting</view>
						<view style="margin-left: auto;margin-right: 10px;"><image src="/icons/arrow_right.png" style="width: 24px;height: 24px;margin-top: 13px;"></image></view>
					</view>
					<view class="functioncard" style="display: flex;">
						<image src="/icons/Shield.png" style="width: 30px;height: 30px;margin-top: 10px;margin-left: 12px;"></image>
						<view style="line-height: 45x;margin-left: 30px;margin-top: 12px;">Privacy</view>
						<view style="margin-left: auto;margin-right: 10px;"><image src="/icons/arrow_right.png" style="width: 24px;height: 24px;margin-top: 13px;"></image></view>
					</view>
					<view class="functioncard" style="display: flex;">
						<image src="/icons/Help circle.png" style="width: 30px;height: 30px;margin-top: 10px;margin-left: 12px;"></image>
						<view style="line-height: 45x;margin-left: 30px;margin-top: 12px;">Help & Feedback</view>
						<view style="margin-left: auto;margin-right: 10px;"><image src="/icons/arrow_right.png" style="width: 24px;height: 24px;margin-top: 13px;"></image></view>
					</view>
				</view>
			</view>
		</view>
	</view>
</template>

<script setup>
	import customTabbarVue from '@/components/customTabbar/customTabbar.vue';
</script>

<style>
	.profile-page{
		height: auto;
		width: 100%;
		background-color: #FDF2C4;
	}
	.more-functions{
		width: 95%;
		height: 200px;
		background-color: #d9d9d9;
		margin-top: 23px;
		margin-left: auto;
		margin-right: auto;
		border-radius: 9px;
		display: flex;
		box-shadow: 0 6rpx 15rpx darkgray;
	}
	.functioncard{
		width: 95%;
		height: 50px;
		background-color: #f0f0f0;
		margin-left: auto;
		margin-right: auto;
		border-radius: 9px;
		margin-top: 12px;
		box-shadow: 0 6rpx 15rpx darkgray;
	}
</style>
