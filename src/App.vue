<template>
	<div class="app">
		1111
		<div class="box">
			{{name}}
		</div>
		<Test />
		<Test />
	</div>
</template>

<script lang='ts'>
	import {
		Component,
		Prop,
		Vue,
		Watch
	} from 'vue-property-decorator';
	import Test from './components/test.vue';

	@Component({
		components:{
			Test
		}
	})
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
