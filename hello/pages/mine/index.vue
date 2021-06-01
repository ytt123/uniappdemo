<template>
	<view>
		<text selectable="true">123123</text>
		<text selectable="true">123123</text>
		<view>
			<text selectable="true">345</text>
		</view>
			<text selectable="true">wwww</text>
			<view></view>
			<text selectable="true">wwww</text>
						<view></view>
			<text selectable="true">123</text>
			
			<view class="box2" hover-class="box2-active">
				<view class="box" hover-class="box-active" hover-stop-propagation> 我是一个盒子</view>
			</view>
			<button size="mini">我是一个按钮</button>
	</view>

</template>

<script>

</script>

<style>
	.box {
		width: 100px;
		height: 100px;
		background-color:#4CD964;
	}
	.box-active {
		background-color: pink;
	}
	.box2 {
		width: 200px;
		height: 200px;
		background-color:red;
	}
	.box2-active {
		background-color:yellow;
	}
</style>
