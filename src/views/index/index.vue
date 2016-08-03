<!--  -->
<template>
<div>

	<group>
	    <x-switch title="默认提示" :value.sync="show1"></x-switch>
	    <x-switch title="文字提示" :value.sync="show2"></x-switch>
	    <x-switch title="提示取消" :value.sync="show3"></x-switch>
	    <x-switch title="提示禁止" :value.sync="show4"></x-switch>
	    <x-switch title="设置出现时间1s" :value.sync="show5"></x-switch>
	    <x-switch title="long text" :value.sync="show6"></x-switch>
	  </group>
	  <toast :show.sync="show1" >默认提示</toast>
	  <toast :show.sync="show2" type="text">处理成功</toast>
	  <toast :show.sync="show3" type="cancel">取消操作</toast>
	  <toast :show.sync="show4" type="warn">禁止操作</toast>
	  <toast :show.sync="show5" :time="1000">1s关闭</toast>
	  <toast :show.sync="show6" type="text" width="20em">Talk is cheap, show me the code.</toast>
	<group>
		<cell title="My Account" value="Protected" is-link></cell>
	</group>
	<h1>123123</h1>
	<divider>默认</divider>
	<x-header>This is the page title.</x-header>
	<divider>不显示后退</divider>
	<x-header :left-options="{showBack: false}">do not show Back</x-header>
	<divider>显示右侧更多</divider>
	<x-header :right-options="{showMore: true}">with more menu</x-header>
	<divider>使用 right 插槽</divider>
	<x-header>with right link<a slot="right">Feedback</a></x-header>
	<divider>自动文字截断</divider>
	<x-header>long long long long long long long ong long long long long long long text<a slot="right">Feedback</a></x-header>
	<divider>使用 left 插槽</divider>
	<x-header>with left slot<a slot="left">Close</a></x-header>
	<divider>更改背景颜色</divider>
	<x-header style="background-color:#000;">custom background color</x-header>
</div>
</template>


<script>
import divider from 'vux/src/components/divider'
import xHeader from 'vux/src/components/x-header'
import group from 'vux/src/components/group'
import cell from 'vux/src/components/cell'
import xSwitch from 'vux/src/components/switch'
import toast from 'vux/src/components/toast'

export default {
	components: {
		divider,
		xHeader,
		group,
		cell,
		xSwitch,
		toast,
	},
	data(){
		return {
			show1: false,
			show2: false,
			show3: false,
			show4: false,
			show5: false,
			show6: false,
		}
	}
}
</script>


<style>
	
</style>