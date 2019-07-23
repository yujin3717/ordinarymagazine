<template>
	<div :id="pagenum" class="page-common swiper-slide full-height-page hide-header" :data-brand-name="databrandNm" data-brand-url="">
		<div class="page-common-inner" data-scrollbar>

			<div class="page-article content-vertical-bottom swiper-lazy" :data-background="background" style="background-size: cover; background-position: center bottom;">
                <div class="spacer" style="height: 334px;"></div>

                <!-- text-block -->
                <div class="text-block animate fadeRight" data-animation style="font-size: 35px; font-weight: 700; color: #fff; line-height: 35px;" v-html="title">
                </div>
                <div class="spacer" style="height: 10px;"></div>
                <!-- text-block -->
                <div class="text-block animate fadeIn" data-animation style="font-size: 15px; color: #fff; line-height: 20px;" v-html="content">
                </div>
                <div class="spacer" style="height: 11px;"></div>
                <!-- text-block -->
                <div class="text-block animate fadeIn" data-animation style="font-size: 14px; color: #fff; line-height: 20px; text-align: right;">{{txt}}</div>
                <div class="spacer" style="height: 50px;"></div>
            </div>

		</div>
	</div>
</template>

<script>
	export default {
		data(){
			return {
				pagenum: 'page-16',
				databrandNm: 'Every is a New Beginning',
				background: 'http://d2bdkorgfosgj9.cloudfront.net/ordinary/vol.27/images/pages/p07/content-1/01.jpg',
				title: `Everyday is<br>
                    a new Beginning`,
                content: `폴 스미스의 유쾌함은 견고했다.<br>
                    그는 늘 새로운 오늘을 살았고<br>
                    앞으로도 그럴 것이다.`,
				txt: 'Editor 이소진',
			}
		}
	}
</script>

<style lang="scss">

</style>
