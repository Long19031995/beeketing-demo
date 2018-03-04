<template>
	<div id="app">
		<Index></Index>
	</div>
</template>

<script>
	import Index from '@/components/Index.vue'
	export default {
		name: 'App',
		components: { Index }
	}
</script>

<style lang="stylus">
	@font-face
		font-family ITCAvantGardeStd
		src url(assets/font/ITCAvantGardeStd-Bk.otf)
	#app
		font-family ITCAvantGardeStd
	.container
		padding 0px 250px
	@media (max-width 768px)
		.container
			padding 0px
</style>