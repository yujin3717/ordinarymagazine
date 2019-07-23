<template>
	<div :id="pagenum" class="page-common swiper-slide panorama-slider-page hide-header" :data-brand-name="databrandNm" data-brand-url="">
		<div class="page-common-inner" data-scrollbar>

			<div class="page-article">
				<!-- panorama-slider -->
				<div class="panorama-slider swiper-container">
					<div class="swiper-wrapper">
						<div class="item swiper-slide">
							<div class="article content-vertical-center" data-swiper-parallax-x="-20%">
								<div class="on-air">{{txt}}</div>
							</div>

							<div class="background-image swiper-lazy" :data-background="background" :style="{'background-position': backgroundP}"></div>
						</div>

						<div class="item swiper-slide">
							<div class="article">
								<div style="height: 32px;"></div>

								<div class="on-air-description"
									 v-html="description"
								>
								</div>
							</div>
						</div>
					</div>
				</div>
				<!-- // panorama-slider -->
			</div>

		</div>
	</div>
</template>

<script>
	export default {
		data(){
			return {
				pagenum: 'page-2',
				databrandNm: '',
				background: 'https://d2bdkorgfosgj9.cloudfront.net/ordinary/vol.27/images/pages/p02/bg-left.jpg',
				backgroundP: 'right bottom',
				description: `<div class="kor">“ 라디오는 생각을 위한 극장이고, 텔레비전은 생각 없는 이들을 위한 극장이다.</div>
									<div class="eng">Radio is the theater of the mind, television is the theater of the mindless.”</div>
									<div class="author">- Steve Allen</div>`,
				txt: 'ON AIR',
			}
		}
	}
</script>

<style lang="scss">

</style>
