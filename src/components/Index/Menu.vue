<template>
	<div id="menu" class="container">
		<div class="logo">
			<img src="@/assets/img/logo.png" alt="logo">
		</div>
		<div class="options">
			<div class="get_started">
				<a href="#">
					Get started
				</a>
			</div>
			<div class="login">
				<a href="#">
					Login
				</a>
			</div>
			<div class="about">
				<a href="#">
					About
				</a>
			</div>
			<div class="princing">
				<a href="#">
					Princing
				</a>
			</div>
			<div class="features active">
				<a href="#">
					Features
				</a>
			</div>
		</div>
		<div class="options-tiny">
			<i class="material-icons icon-bar">reorder</i>
			<div class="list-option">
				<div class="features active">
					<a href="#">
						Features
					</a>
				</div>
				<div class="princing">
					<a href="#">
						Princing
					</a>
				</div>
				<div class="about">
					<a href="#">
						About
					</a>
				</div>
				<div class="login">
					<a href="#">
						Login
					</a>
				</div>
				<div class="get_started">
					<a href="#">
						Get started
					</a>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
	export default {
		name: 'Menu',
		mounted () {
			$('.list-option').hide()
			$('.icon-bar').click(function () {
				$('.list-option').slideToggle('fast')
			})
		}
	}	
</script>

<style lang="stylus" scoped>
	#menu
		height 50px
		box-shadow 0px 0px 20px grey
		.logo
			height 100%
			float left
			padding 10px 0px
			img
				height 100%
		.options
			display block
			line-height 50px
			.features, .princing, .about, .login, .get_started
				float right
				padding 0px 15px
				font-size 12px
				a
					&:hover
						color #0088ff
			a
				text-decoration none
				color #44719f
			.active
				a
					color #0088ff
			.get_started
				a
					background-color #0088ff
					border-radius 3px
					padding 5px
					color white
				&:hover
					a
						color white
		.options-tiny
			display none
			position relative
			width 100%
			z-index 4
			.icon-bar
				float right
				padding 10px
			.list-option
				position absolute
				top 50px
				left 0px
				width 100%
				.features, .princing, .about, .login, .get_started
					float left
					width 100%
					height 30px
					line-height 30px
					padding-left 20px
					font-size 12px
					background-color white
					a
						text-decoration none
						color #44719f
				.active
					a
						color #0088ff
				.features
					border-top 1px solid #ccc
				.get_started
					border-bottom 1px solid #ccc
	@media (max-width 768px)
		.logo
			padding 10px !important
		.options
			display none !important
		.options-tiny
			display block !important
</style>