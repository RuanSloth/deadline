<template>
	<view class="text">
		{{text}}
		
		<div class="setting" v-if="setting">
			<svg t="1667301800348" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg"
				p-id="3395" width="26" height="26">
				<path
					d="M469.333333 60.693333a85.333333 85.333333 0 0 1 85.333334 0l326.826666 188.714667a85.333333 85.333333 0 0 1 42.666667 73.898667v377.386666a85.333333 85.333333 0 0 1-42.666667 73.898667L554.666667 963.306667a85.333333 85.333333 0 0 1-85.333334 0L142.506667 774.592a85.333333 85.333333 0 0 1-42.666667-73.898667v-377.386666a85.333333 85.333333 0 0 1 42.666667-73.898667z m42.666667 73.898667L185.173333 323.306667v377.386666L512 889.408l326.826667-188.714667v-377.386666L512 134.592zM512 341.333333a170.666667 170.666667 0 1 1 0 341.333334 170.666667 170.666667 0 0 1 0-341.333334z m0 85.333334a85.333333 85.333333 0 1 0 0 170.666666 85.333333 85.333333 0 0 0 0-170.666666z"
					fill="#ffffff" p-id="3396"></path>
			</svg>
		</div>
	</view>
	
</template>

<script>
	export default {
		props:{
			text: String,
			setting: {
				type: Boolean,
				default: false
			}
		}
	}
</script>

<style scoped>
	.text{
		padding: 30rpx 0;
		font-size: 46rpx;
		text-align: center;
		color: #fff;
		position: relative;
	}
	.setting{
		position: absolute;
		right: 40rpx;
		top: 30rpx;
	}
</style>