<template>
	<view>
		<customTabbarVue current-menu="Plan"></customTabbarVue>
	</view>
	<view class="plan-page">
		<view style="width: 100%;height: 245px;background-color: #ddffe3;line-height: 200px;">
			<text style="font-size: 36px;margin-left: 30px;">Plan</text>
		</view>
		<view style="width: 100%;height: 100px;background-color: #ccf6ff;border-radius: 70%;margin-top: -70px;text-align: center;padding-top: 45px;font-size: 15px;">
			<view>
				<text>You can try out the basic functions for free, <br>or purchase a plan to access more features.</text>
			</view>
			<view class="plan-card" style="margin-top: 55px;display: flex;">
				<view style="flex: 3;line-height: 250px;margin-left: 18px;"><image src="/icons/Zap.png" style="width: 75px;height: 75px;"></image></view>
				<view style="flex: 7;">
					<view style="margin-top: 15px;"><text style="font-size: 30px;">Monthly Plan</text></view>
					<view style="text-align: left;margin-left: 28px;line-height: 15px;"><text style="font-size: 10px;">-Including all the functions for free users<br>
														 -Provide customized dietary plans<br>
														 -Health check-ups discounts<br>
														 -Monthly settlement</text></view>
					<view style="display: flex;">
						<view style="flex: 2;line-height: 61px;margin-left: 20px;"><image src="/icons/Credit card.png" style="width: 20px;height: 20px;"></image></view>
						<view style="flex: 4.5;font-size: 16px;line-height: 52px;text-align: left;"><text>$2.99/Month</text></view>
						<view style="flex: 3.5;line-height: 90px;text-align: left;"><image src="/icons/Buy.png" style="width: 61px;height: 44px;"></image></view>
					</view>
				</view>
			</view>
			<view class="plan-card" style="margin-top: 20px;display: flex;">
				<view style="flex: 3;line-height: 250px;margin-left: 18px;"><image src="/icons/Zap.png" style="width: 75px;height: 75px;"></image></view>
				<view style="flex: 7;">
					<view style="margin-top: 15px;"><text style="font-size: 30px;">Annual Plan</text></view>
					<view style="text-align: left;margin-left: 28px;line-height: 15px;"><text style="font-size: 10px;">-Including all the functions for free users<br>
														 -Provide customized dietary plans<br>
														 -Health check-ups discounts<br>
														 -Annual settlement</text></view>
					<view style="display: flex;">
						<view style="flex: 2;line-height: 61px;margin-left: 20px;"><image src="/icons/Credit card.png" style="width: 20px;height: 20px;"></image></view>
						<view style="flex: 4.5;font-size: 16px;line-height: 52px;text-align: left;"><text>$29.9/Year</text></view>
						<view style="flex: 3.5;line-height: 90px;text-align: left;"><image src="/icons/Buy.png" style="width: 61px;height: 44px;"></image></view>
					</view>
				</view>
			</view>
			<view style="display: flex;line-height: 16px;margin-top: 22px;margin-left: 19px;">
				<image src="/icons/Info.png" style="width: 16px;height: 16px;"></image>
				<text style="font-size: 8px;margin-left: 8px;">Schools and hospitals can opt for more advanced equipment and plans. </text>
				<text style="font-size: 8px;margin-left: 8px;opacity: 0.2;">more info </text>
			</view>
		</view>
	</view>
</template>

<script setup>
	import customTabbarVue from '@/components/customTabbar/customTabbar.vue';
</script>

<style>
	.plan-page {
		width: 100%;
		height: 100%;
		background-color: #ccf6ff;
	}
	.plan-card{
		width: auto;
		height: 192px;
		background-color: #FFFFFF;
		margin-left: 16px;
		margin-right: 16px;
		border-radius: 8px;
		box-shadow: 0 6rpx 15rpx darkgray;
	}
</style>