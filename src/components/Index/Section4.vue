<template>
	<div id="section3">
		<div class="image">
			<div class="intro">
				<div class="intro1">
					Analyze & Learn their interest on your store
				</div>
				<div class="intro2">
					By analyzing and learning their interests, Beeketing puts you a step ahead of the customer journey to predict products they're most likely to buy.
				</div>
			</div>
			<img src="@/assets/img/arrow-black.png" alt="arrow-black">
			<img src="@/assets/img/device/content3.png" alt="content3">
		</div>
	</div>
</template>

<style lang="stylus" scoped>
	#section3
		float left
		width 100%
		padding 20px 250px 0px 250px
		.image
			padding-top 20px
			.intro
				float left
				width 50%
				padding-top 100px
				.intro1
					font-size 20px
					padding-bottom 20px
					font-weight bold
				.intro2
					font-size 12px
			img:nth-child(2)
				float left
				width 20%
				transform rotate3d(1, 2, 0, 180deg)
			img:nth-child(3)
				float left
				width 30%
	@media (max-width 768px)
		#section3
			padding 20px !important
			.image
				img:nth-child(2)
					margin-bottom 100px !important
			.intro
				padding-top 0px !important	
</style>