<template>
	<div :id="pagenum" class="page-common dual-background-page swiper-slide" :data-brand-name="databrandNm" data-brand-url="">
		<div class="page-common-inner" data-scrollbar>

			<div class="page-common-inner" data-scrollbar>

                <div class="background-image bg-t swiper-lazy" :data-background="contentImg" style="background-position: center bottom;"></div>
                <div class="background-image bg-b swiper-lazy" :data-background="contentImg2" style="background-position: center top;"></div>

            </div>

		</div>
	</div>
</template>

<script>
	export default {
		data(){
			return {
				pagenum: 'page-23',
                databrandNm: 'Every is a New Beginning',
                contentImg: 'https://d2bdkorgfosgj9.cloudfront.net/ordinary/vol.27/images/pages/p07/content-4/01.jpg',
                contentImg2: 'https://d2bdkorgfosgj9.cloudfront.net/ordinary/vol.27/images/pages/p07/content-4/02.jpg',
			}
		}
	}
</script>

<style lang="scss">

</style>
