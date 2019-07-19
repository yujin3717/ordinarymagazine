<template>
    <div :id="pagenum" class="page-common swiper-slide panorama-slider-page animation-page hide-header" :data-brand-name="databrandNm" data-brand-url="">
        <div class="page-common-inner" data-scrollbar>
            <div class="page-article">
                <div class="panorama-slider swiper-container">
                    <div class="swiper-wrapper">
                        <div class="item swiper-slide">
                            <!-- <div class="article">
                                <div class="spacer" style="height: 50px;"></div>

                                
                                <div class="text-block" style="">{{caption}}</div>
                                <div class="spacer" style="height: 0px;"></div>

                               
                                <div class="text-block" style="font-size: 44px; font-weight: 700; line-height: 1.2;">{{title}}</div>
                                <div class="spacer" style="height: 10px;"></div>

                                
                                <div class="text-block" style="letter-spacing: -0.25px;">{{maintext}}</div>
                                <div class="spacer" style="height: 10px;"></div>

                                
                                <div class="text-block" style="font-size: 12px;" v-html="author">
                                    
                                </div>
                                <div class="spacer" style="height: 90px;"></div>
                            </div> -->

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


