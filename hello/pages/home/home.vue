<template>
	<view>
		<text>123{{msg}}</text>
		<text>123{{msg}}</text>
		<view></view>
		<view>
			<image  mode="aspectFit" :src='imgsrc'></image>
		</view>
		<view v-for="(item,index) in arr">
			名字:{{item.name}} 年龄:{{item.age}}
		</view>
		<button type="primary" @click="click('123123')">123</button>
	
	</view>
</template>

<script>
	export default {
		data(){
			return {
				msg:"hello",
				arr:[{name:"ytt",age:15},{name:"ytt",age:15},{name:"ytt",age:15},{name:"ytt",age:15}],
				imgsrc:'http://e.hiphotos.baidu.com/image/pic/item/a1ec08fa513d2697e542494057fbb2fb4316d81e.jpg'
			}
		},
		methods:{
			click:(index)=>{
				console.log('我点击了',index)
			}
		}
	}
</script>

<style>
</style>
