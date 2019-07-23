<template>
    <div :id="pagenum" class="page-common swiper-slide" :data-brand-name="databrandNm" data-brand-url="">
        <div class="page-common-inner" data-scrollbar>

            <div class="page-article">
                <!-- full-image-block -->
                <div class="full-image-block">
                    <img class="swiper-lazy" :data-src="contentImg" alt="" src="">
                </div>
                <div class="full-image-block">
                    <img class="swiper-lazy" :data-src="contentImg2" alt="" src="">
                </div>
                <div class="spacer" style="height: 20px;"></div>

                <!-- text-block -->
                <div class="text-block" v-html="content">
                </div>
                <div class="spacer" style="height: 70px;"></div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data(){
        return{
            pagenum : 'page-20',
            databrandNm: 'Every is a New Beginning',
            contentImg: 'http://d2bdkorgfosgj9.cloudfront.net/ordinary/vol.27/images/pages/p07/content-3/01.jpg',
            contentImg2: 'http://d2bdkorgfosgj9.cloudfront.net/ordinary/vol.27/images/pages/p07/content-3/02.jpg',
            content: `<strong>유쾌하고 진중하게</strong><br>
                        폴 스미스는 유쾌하다. 어떤 자리에서든 누구를 만나든 웃길 준비가 되어 있는 사람 같다. 한국에 방문한 날 그는 단정한 수트에 경쾌한 스트라이프 무늬 양말을 신고 나타났다. 특유의 쾌활함과 위트 넘치는 대화는 주변 사람들을 금세 빠져들게 만든다. 그런 점이 지금까지 자신과 브랜드를 키워 온 원동력이 되었을 것이다. 브랜드의 기본 철학도 ‘위트 있는 클래식’. 80년대에 폴 스미스는 격식은 있어 보이되 남다른 컬러와 디테일을 잘 살려낸 개성 있는 수트를 선보였다. 창의적인 것을 추구하던 영국의 젊고 유능한 남성층에게 그런 점은 충분히 매력적이었다. 그는 점차 유럽, 미국, 아시아 등 국제적으로 사업의 규모를 늘려갔다. 특히 일본에서의 인기는 상상을 뛰어넘는다. 1982년 라이선스 계약을 맺은 이래로 지금까지 일본에만 매장과 아울렛이 200개가 넘는다. 비결을 묻는 말에 그는 “당연히 특별한 이유는 없어요. 열심히 일한 것밖에는”이라고 답한다. 지금까지 그를 있게 한 원동력은 안목과 재능뿐만 아니라 성실함과 꾸준함에 있다. 70대가 된 지금도 매일 아침 6시만 되면 사무실에 출근하고 틈틈이 앨버말 스트리트에 있는 매장을 방문한다. 그는 성공하고 싶다면 꾀를 부리면 안 된다는 것을 잘 알고 있다. 전시장에 소개된 1,500여 점의 디자인과 작품들도 매일 그렇게 사무실과 매장을 오가며 꾸준히 쌓아온 것들이다. 알록달록한 스트라이프 무늬를 입힌 미니 쿠퍼, 에비앙, 라이카 카메라 등 화제를 모았던 컬래버레이션 제품들을 지나면 패션 디자이너의 작업실과 함께 지난 시즌의 의상들이 화려하게 등장한다. 그리고 모든 반세기의 여정은 그가 직접 쓴 쪽지 앞에서 마무리를 맺는다.<br>
                        <br>
                        <strong>“Everyday is a new beginning.”</strong><br>
                        <br>
                        전 세계에 강력한 영향력을 전파하는 폴 스미스. 그가 여전히 현역이라는 사실이 든든하다. 매일이 새로운 시작인 것처럼 폴 스미스는 오늘도 그렇게 살아갈 것이다.`,
        }
    }
}
</script>

<style lang="scss">

</style>


