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
                            <div class="article content-vertical-center" data-swiper-parallax-x="-20%">

                                <div class="dobira-block">
                                    <div class="dobira-block-inner">
                                        <div class="title">{{title}}</div>
                                        <div class="editor">{{txt}}</div>
                                    </div>
                                </div>

                            </div>

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
				background: 'https://d2bdkorgfosgj9.cloudfront.net/ordinary/vol.27/images/pages/p05/open-1@2x.jpg',
                backgroundP: 'right bottom',
                backgroundR: 'https://d2bdkorgfosgj9.cloudfront.net/ordinary/vol.27/images/pages/p05/open-2@2x.jpg',
                backgroundPR: 'left bottom',
				title: '규정하지 않는 음악',
				txt: 'writer 류희성',
			}
		}
	}
</script>

<style lang="scss">

</style>
