<template>
	<div :id="pagenum" class="page-common swiper-slide panorama-slider-page hide-header" :data-brand-name="databrandNm" data-brand-url="">
		<div class="page-common-inner" data-scrollbar>

			<div class="page-article">
				<!-- panorama-slider -->
                <div class="panorama-slider swiper-container">
                    <div class="swiper-wrapper">
                        <div class="item swiper-slide">
                            <div class="background-image swiper-lazy" :data-background="background" :style="{'background-position': backgroundP}"></div>
                        </div>

                        <div class="item swiper-slide">
                            <div class="background-image swiper-lazy" :data-background="backgroundR" :style="{'background-position': backgroundPR}"></div>
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
				pagenum: 'page-7',
				databrandNm: '규정하지 않는 음악',
				background: 'https://d2bdkorgfosgj9.cloudfront.net/ordinary/vol.27/images/pages/p05/panorama-01.jpg',
                backgroundP: 'right bottom',
                backgroundR: 'https://d2bdkorgfosgj9.cloudfront.net/ordinary/vol.27/images/pages/p05/panorama-02.jpg',
                backgroundPR: 'left bottom'
			}
		}
	}
</script>

<style lang="scss">

</style>
