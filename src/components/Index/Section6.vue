<template>
	<div id="section6">
		<div class="text1">
			Ready to Get Started?
		</div>
		<button class="view_more">
			view more apps
		</button>
		<hr>
		<div class="text2">
			E-marketing apps that give every sellers <b>the POWER</b>
			<br>
			to sell effectively like Amazon
		</div>
		<div class="slider">
			<div class="prev">
				<i class="material-icons">chevron_left</i>
			</div>
			<div class="list-item">
				<div class="item">
					<div class="icon">
						<img src="@/assets/img/scvsoft-logo.png" alt="">
					</div>
					<div class="text-slider1">
						"Beeketing has increase our conversion rate by 23% and bring back the lost revenue with in just a couple of weeks. The extra sales has paid for the app itself for the whole year!
						<br>
						Definitely recommended!"
					</div>
					<div class="text-slider2">
						Helen Jones
					</div>
					<div class="text-slider3">
						FOUNDER OF AVIVA BOUTIQUE
					</div>
				</div>
			</div>
			<div class="next">
				<i class="material-icons">chevron_right</i>
			</div>
		</div>
	</div>
</template>

<style lang="stylus" scoped>
	#section6
		float left
		padding 20px 250px
		width 100%
		text-align center
		.text1
			width 100%
			font-weight bold
			font-size 18px
			padding-bottom 20px
		button.view_more
			padding 15px 30px
			background-color #12ca64
			color white
			border none
			outline none
			border-radius 5px
			font-size 17px
			margin-bottom 50px
		.text2
			font-size 18px
		.slider
			.prev, .list-item, .next
				float left
			.prev, .next
				padding-top 50px
				width 100px
				i
					font-size 50px
			.list-item
				width calc(100% - 200px)
				.item
					.icon
						height 100px
						img
							height 100%
					.text-slider1
						font-size 14px
						padding-bottom 20px
					.text-slider2
						font-size 17px
						padding-bottom 10px
						color #006ae2
					.text-slider3
						font-size 14px
	@media(max-width 768px)
		#section6
			padding 20px 0px !important
			.slider
				.prev, .next
					width 35px
			.list-item
				width calc(100% - 70px) !important
</style>