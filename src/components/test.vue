<template>
	<div>
        {{num}}
        <button @click="add">add</button>
	</div>
</template>

<script lang='ts'>
	import {
		Component,
		Prop,
		Vue,
		Watch
    } from 'vue-property-decorator';
    
    @Component
	export default class Test extends Vue {
		public num:number  = 0;
        add(){
            let num = this.num 
            this.num = ++num
            console.error(this.num,this)
        }
	
	}
</script>

<style lang="less">
	
</style>
