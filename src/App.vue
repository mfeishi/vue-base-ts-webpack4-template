<template>
	<div class="app">
		1111
		<div class="box">
			{{name}}
		</div>
		
	</div>
</template>

<script lang='ts'>
	import {
		Component,
		Prop,
		Vue,
		Watch
	} from 'vue-property-decorator';

	export default class App extends Vue {
		private name:string  = 'template';
		private isShowNav:boolean = true;
		mounted(){
			console.error('mmm')
		}
	
	}
</script>

<style lang="less">
	.app{
		.box{
			background: lavender;
		}
		
	}
</style>
