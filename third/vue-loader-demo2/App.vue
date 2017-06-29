<template>
	<h1>welcome Vue</h1>
	<h2 @click="change">{{msg}}</h2>
	<my-menu></my-menu>
</template>
<script>
import Menu from './components/Menu.vue'

		export default{
			data(){
				return {
					msg:'haha'
				}
			},
			methods:{
				change(){
					this.msg="哇哈哈"
				}
			},
			components:{
				'my-menu':Menu
			}
		}
</script>
<style>
	body{
		background:#ccc;
	}
</style>