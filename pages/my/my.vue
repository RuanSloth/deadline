<template>
	<view class="all bg">
		<view class="">
			<NavBar :text="title"></NavBar>
		</view>
	</view>


</template>

<script>
	import NavBar from '@/component/NavBar.vue'
	export default {
		data() {
			return {
				title: '我的'
			};
		},
		components: {
			NavBar
		},
		methods: {

		}
	}
</script>

<style>
	.bg {
		background-image: url('../../static/bg.jpg');
		background-size: cover;
		background-repeat: no-repeat;

	}

	.all {
		height: 100vh;
	}
</style>
