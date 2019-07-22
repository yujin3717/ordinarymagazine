<template>
    <div :id="pagenum" class="page-common swiper-slide full-height-page hide-header" :data-brand-name="databrandNm" data-brand-url="">
        <div class="page-common-inner" data-scrollbar>

            <div class="page-article swiper-lazy" :data-background="background">
                <div class="body">
                    <div class="title" v-html="title"></div>
                    <div class="button" v-html="button"></div>
                </div>

                <div class="foot">
                    <div class="contact">
                        <div class="common text" v-html="footTitle"></div>
                        <div class="common email" v-html="footEmail"></div>
                        <div class="common homepate" v-html="footHomepage"></div>
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
            pagenum: 'last-cover',
            databrandNm: 'CLOSING',
            background: 'http://ordinary.dev.tebah.media/vol.27/images/cover/lastcover.jpg',
            title: '매거진을 평가해주세요',
            button: `<a href="https://forms.gle/mVU8X3oD5PiQyZBL7" target="_blank" rel="noopener noreferrer">참여하기 <i class="cuscon-ios-arrow-right"></i></a>`,
            footTitle: '광 고 문 의',
            footEmail: `<a href="mailto:mackerki@monkeylab.co.kr" target="_blank" rel="noopener noreferrer">mackerki@monkeylab.co.kr</a>`,
            footHomepage: `<a href="http://magazineordinary.com/" target="_blank" rel="noopener noreferrer">http://magazineordinary.com/</a>`
        }
    }
}
</script>

<style lang="scss">
    #last-cover {
        .page-article {
            display: flex;
            flex-direction: column;
            color: #fff;
            text-align: center;

            .body {
                flex: 1;
                display: flex;
                flex-direction: column;
                justify-content: center;
                align-items: center;

                .title {
                    font-size: 30px;
                    font-weight: 700;
                }

                .button {
                    margin-top: 20px;

                    a {
                        display: inline-flex;
                        justify-content: center;
                        align-items: center;
                        width: 152px;
                        height: 40px;
                        font-size: 16px;
                        background-color: #526c41;
                        border-radius: 33px;
                    }
                }
            }

            .foot {
                flex: 0;
                padding: 30px 0;

                .common {
                    margin-top: 10px;

                    &:first-child {
                        margin-top: 0;
                    }
                }
            }
        }
    }
</style>


