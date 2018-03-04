<template>
	<div id="section8">
		<div class="text1">
			Ready to increase your sales by 20%+ ?
		</div>
		<div class="text2">
			No sales team, no marketers, no engineers. Just results & Beeketing.
		</div>
		<button class="get_started">
			Get started now
		</button>
		<div class="footer">
			<div class="btn-group">
				<button class="active">
					Blog
				</button>
				<button>
					Press kit
				</button>
				<button>
					Careers
				</button>
				<button>
					Contact
				</button>
			</div>
			<div class="social">
				facebook... twitter...
			</div>
			<br>
			<div class="contact-text">
				Contact Us | © Beeketing 2015. All rights reserved.
			</div>
		</div>
	</div>
</template>

<style lang="stylus" scoped>
	#section8
		float left
		width 100%
		background-image url(../../assets/img/footer/background-footer.png)
		background-color #022e71
		background-blend-mode multiply
		background-position 0px -200px
		background-size cover
		color white
		text-align center
		.text1
			font-size 30px
			padding-top 50px
			padding-bottom 10px
		.text2
			font-size 12px
			padding-bottom 70px
		button.get_started
			border none
			outline none
			border-radius 3px
			padding 15px 30px
			background-color #fb1ca4
			color white
			margin-bottom 100px
			&:hover
				cursor pointer
		.footer
			padding-bottom 50px
			.btn-group
				display flex
				justify-content center
				button
					background-color #071130
					outline none
					border none
					padding 10px 20px
					color white
					&:hover
						cursor pointer
					&.active
						color #0088ff
				button:nth-child(1)
					border-radius 5px 0px 0px 5px
				button:last-child
					border-radius 0px 5px 5px 0px
			.social
				padding-top 50px
			.contact-text
				font-size 12px
	@media(max-width 768px)
		#section8
			padding 10px
</style>