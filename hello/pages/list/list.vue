<template>
	<view>
		<view>这是列表页</view>
		<view></view>
		<view class="box-item" v-for="item in arr">
			{{item}}
		</view>
		<view>
	      <button @click='refsh'>我要刷新</button>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				arr:[]
			}
		},
		onPullDownRefresh(){  
			console.log('我要刷新了')
			setTimeout(()=> {
				this.arr=["ios","android","java","react","vue","ios","android","java","react","vue","ios","android","java","react","vue"]
				uni.stopPullDownRefresh()
			}, 2000);
			
		},
		onReachBottom() {
			console.log('触底了')
			// this.arr.push('qwe')
			setTimeout(()=>{
				this.arr=[...this.arr,...['123','456']]
			console.log('增加了')
			},2000)
			
		},
		methods: {
			refsh:function(){
				uni.startPullDownRefresh({
					
				})
			}
		}
	}
</script>

<style>
.box-item{
	width: 100rpx;
	height: 200rpx;
	background-color:#007AFF ;
}
</style>
