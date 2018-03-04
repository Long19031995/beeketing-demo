<template>
	<div id="section2" class="container">
		<div class="text">
			Helping more than <b>6,000 online sellers</b> to sell to millions of customers
		</div>
		<div class="list_logo">
			<div class="prev">
				<i class="material-icons">chevron_left</i>
			</div>
			<div class="list_logo-img">
				<div v-for="logo in listLogo" class="logo-img">
					<img :src="logo.src">
				</div>
			</div>
			<div class="next">
				<i class="material-icons">chevron_right</i>
			</div>
		</div>
		<div class="illustration">
			<div class="topic_slide">
				<div class="arrow">
					<img src="@/assets/img/arrow-white.png" alt="">
				</div>
				<div class="slide">
					<div class="prev">
						<i class="material-icons">chevron_left</i>
					</div>
					<div class="list-topic">
						<div v-for="topic in listTopic" class="topic">
							<div class="topic1">
								{{ topic.content1 }}
							</div>
							<div class="topic2">
								{{ topic.content2 }}
							</div>
						</div>
					</div>
					<div class="next">
						<i class="material-icons">chevron_right</i>
					</div>
				</div>
			</div>
			<div class="image">
				<div class="ip6-black">
					<img src="@/assets/img/device/ip6-black.png" alt="ip6-black">
				</div>
				<div v-for="content in listContent" class="list_image-topic">
					<img :src="content.src" :alt="content.alt">
				</div>
			</div>
		</div>
	</div>
</template>

<script>
	export default {
		name: 'Section2',
		data () {
			return {
				listLogo: [
					{
						src: require('@/assets/img/list-logo/logo-app-1.png'),
						alt: 'logo-app-1'
					},
					{
						src: require('@/assets/img/list-logo/logo-app-2.png'),
						alt: 'logo-app-2'
					},
					{
						src: require('@/assets/img/list-logo/logo-app-3.png'),
						alt: 'logo-app-3'
					},
					{
						src: require('@/assets/img/list-logo/logo-app-4.png'),
						alt: 'logo-app-4'
					},
					{
						src: require('@/assets/img/list-logo/logo-app-5.png'),
						alt: 'logo-app-5'
					}
				],
				listContent: [
					{
						src: require('@/assets/img/device/content1.png'),
						alt: 'content1'
					}
				],
				listTopic: [
					{
						content1: 'Personalized recommendation'
					},
					{
						content2: 'Recommend products customers want'
					}
				]
			}
		}
	}
</script>
<style lang="stylus" scoped>
	#section2
		padding-top 30px
		padding-bottom 30px
		.text
			float left
			width calc(100% - 250px)
			font-size 14px
			text-align center
		.list_logo
			float left
			width calc(100% - 250px)
			height 60px
			line-height 60px
			margin 20px 0px
			padding-right 20px
			.prev, .list_logo-img, .next
				float left
				height 100%
			.prev, .next
				width 24px
				color #b2b2b2
				line-height inherit
				&:hover
					cursor pointer
			.list_logo-img
				width calc(100% - 48px)
				overflow hidden
				display flex
				flex-wrap nowrap
				.logo-img
					float left
					height 100%
					img
						height 100%
		.illustration
			float left
			width 250px
			.topic_slide
				position relative
				width 120%
				z-index 3
				top -250px
				left -130%
				.arrow
					width 100%
					float left
					img
						float right
						width 50%
				.slide
					width 100%
					.prev, .list-topic, .next
						float left
					.prev, .next
						width 10px
						color white
						font-size 30px
						&:hover
							cursor pointer
					.list-topic
						width calc(100% - 20px)
						text-align center
						font-size 12px
						.topic1
							color #0181f2
							font-style italic
						.topic2
							color white
			.image
				position relative
				width 100%
				z-index 2
				top -400px
				.ip6-black
					width 100%
					position absolute
					top 0px
					img
						width 100%
				.list_image-topic
					position absolute
					width 100%
					top 0px
					img
						position absolute
						top 55px
						left 16px
						width calc(100% - 30px)
	@media (max-width 768px)
		.text
			width 100% !important
			padding 0px 50px
		.list_logo
			width 100% !important
			padding-right 0px !important
		.illustration
			width 100% !important
			.topic_slide
				width 50% !important
				top 150px !important
				left 0px !important
				padding 0px 10px
				.topic1, .topic2
					font-size 10px
				.topic2
					color black !important
				.prev, .next
					color black !important
			.image
				width 50% !important
				top 0px !important
				left 50%
				.list_image-topic
					img
						top 35px !important
						left 11px !important
						width calc(100% - 22px) !important
</style>