<template>
	<view class="all bg">
		<view class="">
			<NavBar :text="title" :setting="true"></NavBar>
		</view>
		<add></add>
		</div>
	</view>
</template>

<script>
	import NavBar from '@/component/NavBar.vue'
	import add from '@/component/add.vue'
	export default {
		data() {
			return {
				title: '正计时'
			};
		},
		components: {
			NavBar,add
		},
		methods: {

		}
	}
</script>

<style lang="less">
.bg {
		background-image: url('../../static/bg.jpg');
		background-size: cover;
		background-repeat: no-repeat;

	}

	.all {
		height: 100vh;
	}
</style>
