<template>
	<view class="all bg">
		<view class="">
			<NavBar :text="title" :setting="true"></NavBar>
		</view>
		
		<add @click.native="toAdd"></add>
	</view>

</template>

<script>
	import NavBar from '@/component/NavBar.vue'
	import add from '@/component/add.vue'
	export default {
		data() {
			return {
				title:'倒计时'
			};
		},
		components:{
			NavBar,add
		},
		methods:{
			toAdd(){

				uni.navigateTo({
					url: '../../pages/addDo/addDo'
				});
			}
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
