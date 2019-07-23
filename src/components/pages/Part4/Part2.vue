<template>
    <div :id="pagenum" class="page-common swiper-slide" :data-brand-name="databrandNm" data-brand-url="">
        <div class="page-common-inner" data-scrollbar>

            <div class="page-article">
                <!-- full-image-block -->
                <div class="full-image-block">
                    <img class="swiper-lazy" :data-src="contentImg" alt="">
                </div>
                <div class="full-image-block">
                    <img class="swiper-lazy" :data-src="contentImg2" alt="">
                </div>
                <div class="spacer" style="height: 20px;"></div>

                <!-- text-block -->
                <div class="text-block" v-html="content">
                </div>
                <div class="spacer" style="height: 30px;"></div>
            </div>

            <div class="page-article">
                <!-- full-image-block -->
                <div class="full-image-block">
                    <img class="swiper-lazy" :data-src="contentImg3" alt="">
                </div>
                <div class="spacer" style="height: 20px;"></div>

                <!-- text-block -->
                <div class="text-block" v-html="content2">
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
            pagenum : 'page-14',
            databrandNm: '음악 맛집',
            contentImg: 'http://d2bdkorgfosgj9.cloudfront.net/ordinary/vol.27/images/pages/p06/c06.jpg',
            contentImg2: 'http://d2bdkorgfosgj9.cloudfront.net/ordinary/vol.27/images/pages/p06/c07.jpg',
            contentImg3: 'http://d2bdkorgfosgj9.cloudfront.net/ordinary/vol.27/images/pages/p06/c08.jpg',
            content: `<strong>르 캬바레 도산</strong><br>
                    19세기 말에서 20세기 초, 예술적 낭만이 온 거리를 수놓았던 벨 에포크La Belle poque 시대에는 문인들과 예술가와 같은 지성인 집단이 한데 모여 미식과 유흥을 즐기던 ‘캬바레cabaret’라는 문화가 존재했다. 이를 현대적으로 재해석한 샴페인 라운지, 르 캬바레 도산은 강남의 한복판인 도산대로에 자리한다. 들어서자마자 눈길을 사로잡는 샹들리에는 마치 궁전에 입성한 귀족이 된 것만 같은 착각에 빠질 만큼 화려하다. 이곳만의 특별한 점은 바로 천장이 완전히 열리는 개폐식 돔형 지붕이다. 여름 저녁, 탁 트인 전경과 더불어 매월마다 새롭게 제철 식자재로 메뉴를 구성한 프렌치 코스 요리 한상차림과 엄선한 샴페인을 즐길 수 있다.`,
            content2: `빅투아 샴페인과 잘 어울리는 ‘브리야 사바랭과 파인애플 크뢰메’를 단품 메뉴로 추천한다. 트리플 크림치즈의 여왕과 달콤한 크뢰메의 조합은 매우 부드러운 질감과 깔끔한 끝맛을 자랑한다. 저녁 9시 이전에는 차분히 대화를 나누며 디너를 즐기고자 하는 고객들이 대부분인 만큼, 잔잔한 프랑스 음악을 선곡한다. 이후엔 딥 하우스, 트로피칼 하우스, 테크 하우스 등 분위기를 고조시킬 수 있는 하우스 음악이 흘러나온다. 뉘엿뉘엿 넘어가는 석양과 하늘을 바라보며 요리와 음악을 즐길 수 있는 르 캬바레 도산은 바쁜 일상에 지친 이들을 위한 색다른 휴식처다.`
        }
    }
}
</script>

<style lang="scss">

</style>


