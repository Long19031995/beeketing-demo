<template>
	<div id="section1">
		<div class="background">
			<img src="@/assets/img/bg-section1.jpg" alt="background">
			<div class="background-mask"></div>
		</div>
		<div class="foreground container">
			<div class="text">
				Your customers all behave differently, why treat them all the same?
			</div>
			<button class="get_started_now-btn">
				Get started now
			</button>
		</div>
	</div>
</template>

<style lang="stylus" scoped>
	#section1
		position relative
		height 400px
		.background
			position absolute
			z-index 1
			width 100%
			height 100%
			overflow hidden
			img
				position absolute
				z-index 1
				top -150px
				left 0px
				width 100%
			.background-mask
				position absolute
				z-index 2
				top 0px
				left 0px
				width 100%
				height 100%
				background-color #022e71
				opacity 0.8
				mix-blend-mode multiply
		.foreground
			position absolute
			z-index 2
			width 100%
			height 100%
			display flex
			flex-direction column
			justify-content center
			.text
				color white
				font-size 12px
			button.get_started_now-btn
				width 130px
				padding 10px 0px
				margin-top 10px
				background-color #0088ff
				outline none
				border none
				color white
				border-radius 3px
				&:hover
					cursor pointer
	@media (max-width 768px)
		#section1
			height 150px
			.background
				img
					top 0px !important
			.foreground
				.text
					text-align center
					padding 0px 50px
				button.get_started_now-btn
					margin 10px auto 0px auto
</style>