<template>
	<div id="index-page">
		<Menu></Menu>
		<Section1></Section1>
		<Section2></Section2>
		<Section3></Section3>
		<Section4></Section4>
		<Section5></Section5>
		<Section6></Section6>
		<Section7></Section7>
		<Section8></Section8>
	</div>
</template>

<script>
	import Menu from '@/components/Index/Menu.vue'
	import Section1 from '@/components/Index/Section1.vue'
	import Section2 from '@/components/Index/Section2.vue'
	import Section3 from '@/components/Index/Section3.vue'
	import Section4 from '@/components/Index/Section4.vue'
	import Section5 from '@/components/Index/Section5.vue'
	import Section6 from '@/components/Index/Section6.vue'
	import Section7 from '@/components/Index/Section7.vue'
	import Section8 from '@/components/Index/Section8.vue'
	export default {
		name: 'index-page',
		components: { Menu, Section1, Section2, Section3, Section4, Section5, Section6, Section7, Section8 }
	}
</script>

<style lang="stylus" scoped>
	#index-page
		background-color white
</style>