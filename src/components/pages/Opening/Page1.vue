<template>
	<div :id="pagenum" class="page-common swiper-slide panorama-slider-page hide-header" :data-brand-name="databrandNm" data-brand-url="">
		<div class="page-common-inner" data-scrollbar>

			<div class="page-article">
				<div class="panorama-slider swiper-container">
					<div class="swiper-wrapper">
						<div class="item swiper-slide">
							<div class="background-image swiper-lazy" :data-background="background" v-bind:style="{ 'background-position': backgroundP }"></div>
						</div>

						<div class="item swiper-slide">
							<div class="article content-vertical-center" data-swiper-parallax-x="-20%">

								<!-- text-block -->
								<div
									class="text-block"
									style="font-size: 30px; font-weight: 700; font-style: italic; color: #fff; text-align: center;"
									v-html="tit"
								>
								</div>
								<div class="spacer" style="height: 12px;"></div>

								<!-- text-block -->
								<div
									class="text-block"
									style="font-size: 20px; font-weight: 700; color: #fff; line-height: 25px; text-align: center;"
									v-html="txt"
								>
								</div>
								<div class="spacer" style="height: 0;"></div>

							</div>

							<div class="background-image swiper-lazy" :data-background="background2" v-bind:style="{ 'background-position': background2P }"></div>
						</div>
					</div>
				</div>
			</div>

		</div>
	</div>
</template>

<script>
	export default {
		data(){
			return {
				pagenum: 'page-1',
				databrandNm: 'Opening',
				background: 'https://d2bdkorgfosgj9.cloudfront.net/ordinary/vol.27/images/pages/p01/bg-left.jpg',
				backgroundP: 'right bottom',
				background2: 'https://d2bdkorgfosgj9.cloudfront.net/ordinary/vol.27/images/pages/p01/bg-right.jpg',
				background2P: 'left bottom',
				tit: 'LIVE',
				txt: '살아있음을 느끼게 하는<br>모든 것들에 대한 찬사',
			}
		}
	}
</script>

<style lang="scss">

</style>
