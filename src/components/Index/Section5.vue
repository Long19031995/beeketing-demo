<template>
	<div id="section5">
		<div class="text">
			<div class="text1">
				Smart Marketing Apps to turn your visitors into revenue
			</div>
			<div class="text2">
				From the data collected, we build a platform of smart marketing apps to follow visitors right when they step on your store and gradually convert them to customers - then loyal customers for you.
			</div>
		</div>
		<img src="@/assets/img/device/content4.png" alt="content4">
		<div class="slider">
			<div class="prev">
				<i class="material-icons">chevron_left</i>
			</div>
			<div class="list-item">
				<div v-for="item in listItem" :class="item.class">
					<div class="icon">
						<img :src="item.icon" :alt="item.icon">
					</div>
					<div class="text">
						<div class="text1">
							{{ item.text1 }}
						</div>
						<div class="text2">
							{{ item.text2 }}
						</div>
					</div>
					<button class="learn_more">
						Learn more
					</button>
				</div>
			</div>
			<div class="next">
				<i class="material-icons">chevron_right</i>
			</div>
		</div>
	</div>
</template>

<script>
	export default {
		name: 'Section5',
		data () {
			return {
				listItem: [
					{
						icon: require('@/assets/img/icon-item1.png'),
						text1: 'Better Coupon Box',
						text2: 'Popup a coupon box to turn visitors into social followers, email subscribers and increase your sales.',
						class: 'item'
					},
					{
						icon: require('@/assets/img/icon-item2.png'),
						text1: 'Product Recommendation',
						text2: 'Target recommendations to the right customers around their shopping journey on your site.',
						class: 'item active'
					},
					{
						icon: require('@/assets/img/icon-item3.png'),
						text1: 'Email automation',
						text2: 'Follow up your customers with automated emails personalized to their behavior.',
						class: 'item'
					}
				]
			}
		}
	}
</script>
<style lang="stylus" scoped>
	#section5
		float left
		text-align center
		width 100%
		background-color #ececec
		padding 30px 350px
		> .text
			color #383838
			.text1
				font-size 20px
				font-weight bold
				padding-bottom 30px
			.text2
				font-size 12px
				padding-bottom 50px
		> img
			width 100%
			margin-bottom 30px
		.slider
			width 100%
			.prev, .list-item, .next
				float left
			.prev
				margin-left -100px
				margin-top 100px
				&:hover
					cursor pointer
				i
					font-size 100px
					color #797979
			.next
				margin-right -100px
				margin-top 100px
				&:hover
					cursor pointer
				i
					font-size 100px
					color #797979
			.list-item
				display flex
				.item
					background-color white
					border-radius 5px
					padding 10px
					margin 10px
					opacity 0.5
					transform scale(0.8)
					&.active
						opacity 1
						transform scale(1.0)
					.icon
						margin-top -30px
						img
							width 60px
							height 60px
							box-shadow 0px 0px 5px grey
							border-radius 5px
					.text
						.text1
							font-size 14px
							font-weight bold
							margin-top 20px
						.text2
							font-size 10px
							margin-top 20px
							margin-bottom 50px
					button.learn_more
						border none
						outline none
						border-radius 3px
						background-color #2b9cff
						color white
						padding 10px 0px
						width 80%
						font-size 12px
						box-shadow 0px 5px 10px #ccc
						margin-bottom 15px
						&:hover
							cursor pointer
	@media (max-width 768px)
		#section5
			padding 0px !important
</style>