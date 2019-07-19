<template>
    <div :id="pagenum" class="page-common swiper-slide panorama-slider-page animation-page hide-header" :data-brand-name="databrandNm" data-brand-url="">
        <div class="page-common-inner" data-scrollbar>
            <div class="page-article">
                <div class="panorama-slider swiper-container">
                    <div class="swiper-wrapper">
                        <div class="item swiper-slide">
                            <div class="background-image swiper-lazy" :data-background="imgbackground" style="background-position: right top;"></div>
                        </div>

                        <div class="item swiper-slide">
                            <div class="article content-vertical-bottom">
                            </div>

                            <div class="background-image swiper-lazy" :data-background="imgbackground2" style="background-position: left top;"></div>
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
            pagenum : 'page-1',
            databrandNm: 'Opening',
            imgbackground: 'http://ordinary.dev.tebah.media/images/open/open-1@1x.png',
            imgbackground2: 'http://ordinary.dev.tebah.media/images/open/open-2@1x.png'
        }
    }

}
</script>

<style lang="scss">

</style>


