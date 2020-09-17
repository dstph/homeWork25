<template>
	<div class="form">
		<input v-for="(item, index) in form" :key="item.index" :id="index" :type="item.substr(11).replace(']', '')" v-model="model[index]" >	
		<span></span>
    </div>
</template>

<script>
	export default{
		props: ['form','model']
	}
</script>

<style>
input{
	display: block;
	margin: 5px;
}

</style>
	

