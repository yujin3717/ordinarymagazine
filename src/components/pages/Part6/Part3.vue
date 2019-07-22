<template>
    <div :id="pagenum" class="page-common full-height-page swiper-slide" :data-brand-name="databrandNm" data-brand-url="">
        <div class="page-common-inner" data-scrollbar>
            <div class="page-article">
                <!-- full-image-block -->
                <div class="full-image-block">
                    <img class="swiper-lazy" :data-src="Img" alt="">
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data(){
        return{
            pagenum : 'page-27',
            databrandNm: '하루키와 맥주',
            Img: 'http://ordinary.dev.tebah.media/vol.27/images/pages/p08/02.jpg'
        }
    }
}
</script>

<style lang="scss">

</style>


