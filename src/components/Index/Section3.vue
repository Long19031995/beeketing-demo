<template>
	<div id="section3">
		<div class="text">
			<div class="text1">
				How it works
			</div>
			<br>
			<a href="#">
				play video intro
				<i class="material-icons">play_circle_outline</i>
			</a>
		</div>
		<div class="image">
			<img src="@/assets/img/device/content2.png" alt="content2">
			<img src="@/assets/img/arrow-black.png" alt="arrow-black">
			<div class="intro">
				<div class="intro1">
					Track your customers' bahavior
				</div>
				<div class="intro2">
					Every visit your store gets real person. Beeketing helps you see who they are, know what they do on the store.
				</div>
			</div>
		</div>
	</div>
</template>

<style lang="stylus" scoped>
	#section3
		float left
		width 100%
		background-color #ececec
		padding 20px 250px 0px 250px
		.text
			text-align center
			.text1
				font-size 40px
				color #383838
			a
				text-transform uppercase
				text-decoration none
				color #0088ff
		.image
			padding-top 20px
			img:nth-child(1)
				width 40%
			img:nth-child(2)
				width 20%
				margin-bottom 200px
				margin-left -25px
			.intro
				float right
				width 40%
				padding-top 80px
				.intro1
					font-size 20px
					padding-bottom 20px
					font-weight bold
				.intro2
					font-size 12px
	@media (max-width 768px)
		#section3
			padding 20px !important
			margin-top 250px
			.image
				img:nth-child(2)
					margin-bottom 100px !important
			.intro
				padding-top 0px !important
					
</style>