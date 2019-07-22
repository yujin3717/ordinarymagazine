<template>
    <div :id="pagenum" class="page-common swiper-slide" :data-brand-name="databrandNm" data-brand-url="">
        <div class="page-common-inner" data-scrollbar>

            <div class="page-article">
                <!-- full-image-block -->
                <div class="full-image-block">
                    <img class="swiper-lazy" :data-src="titelImg" alt="">
                </div>
                <div class="spacer" style="height: 30px;"></div>

                <!-- text-block -->
                <div class="text-block" style="font-size: 15px; font-weight: 700; color: #343434; line-height: 26px;" v-html="titletxt">
                </div>
                <div class="spacer" style="height: 30px;"></div>

                <!-- text-block -->
                <div class="text-block" v-html="content">
                </div>
                <div class="spacer" style="height: 30px;"></div>
            </div>

            <div class="page-article">
                <!-- full-image-block -->
                <div class="full-image-block">
                    <img class="swiper-lazy" :data-src="contentImg" alt="">
                </div>
                <!-- full-image-block -->
                <div class="full-image-block">
                    <img class="swiper-lazy" :data-src="contentImg2" alt="">
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
            pagenum : 'page-13',
            databrandNm: '음악 맛집',
            titelImg: 'http://ordinary.dev.tebah.media/vol.27/images/pages/p06/c01.jpg',
            titletxt: `일정 수준의 이상의 맛과 재미를 동시에 만족하는 공간은 흔하지 않다.<br>
                    까다로운 취향을 가진 이를 만족시켜줄 독창적이면서도 색다른 공간 네 곳.`,
            contentImg: 'http://ordinary.dev.tebah.media/vol.27/images/pages/p06/c02.jpg',
            contentImg2: 'http://ordinary.dev.tebah.media/vol.27/images/pages/p06/c03.jpg',
            content: `<strong>청담 겟올라잇</strong><br>
                    과거 서울 청담동은 대한민국 상류층의 문화 발상지 중 하나로 최신 트렌드가 살아 숨쉬는 동네였다. 그러나 현재는 화려한 헤어숍과 럭셔리 부티크가 가득한 곳으로만 인식되고 있다. 이런 천편일률적이면서도 어딘지 모르게 딱딱하고 불편한 청담동 특유의 분위기 속에서, 즐겁고 신나는 공연을 지향하는 겟올라잇은 분명 이제까지 보던 여타 라운지 계열의 장소들과는 결을 달리 한다. 어떤 곳에 있더라도 무대를 볼 수 있도록 자리를 배치했고, 조명과 인테리어의 세심한 디테일 구성이 돋보인다. 공연 중에는 사운드 엔지니어가 태블릿 컴퓨터를 들고 구석구석을 돌아다니며 실시간으로 점검하는 등 음향에 많은 신경을 쏟고 있다. 클래식, 재즈, 퓨전음악 등 장르의 제한을 두지 않고 관객과 소통할 수 있는 다양한 공연을 선보인다. 또한 무대 연출이나 프로그램 구성에 심혈을 기울이고 있는 만큼 공연에 대한 만족도가 높아 주말에는 테이블 예약이 힘들 정도로 열광적인 호응을 이끌어내고 있다. 국내외 수많은 대회에서 입상한 바텐더들이 서빙을 해주는 칵테일 또한 특별하다. 겟올라잇에서만 맛볼 수 있는 여름 한정 시그니처 칵테일 ‘가든 브리즈’는 럼에 저온 숙성한 파인애플을 넣어 완성해 민트의 상쾌함과 열대과일의 달콤함을 동시에 즐길 수 있다.`,
            content2: `<strong>바 81</strong><br>
                    서울의 밤은 화려하다. 이 매혹적인 도시의 야경을 즐길 수 있는 샴페인 전문 바인 바 81은 국내 최고층 건물인 롯데월드타워 81층에 있다. 강남 전체를 조망할 수 있고 천천히 흐르는 한강이 한눈에 내려다 보이는 전망은 그 어떤 라운지에서도 찾기 힘든 경험을 선사한다. 샴페인의 버블을 형상화한 화려한 샹들리에, 샹파뉴 지역의 테루아를 표현한 석회암 벽면 등의 디자인을 통해 특별한 정체성을 표현했다. 압도적인 2층 높이의 샴페인&와인 셀러는 보는 이들로 하여금 감탄을 자아내게 한다. 자유롭고 낭만적인 프렌치 감성의 모던 하우스 음악이 주로 흘러나오며, 금요일과 토요일 밤에는 디제잉을 통해 부드럽고 로맨틱하면서도 설렘 가득한 분위기를 연출한다. 미쉐린 3스타 야닉 알레노 셰프의 현대적인 파리지앵 메뉴를 선보이는데, 그중 ‘비프 타르타르와 푸아그라 파르페’는 소뼈 용기 안에 빼곡히 채워 넣어 프랑스 요리의 이국적인 맛을 살린 이곳의 시그니처 메뉴다. 바 81은 샴페인바라는 특성에 걸맞게 다양한 RM(Recoltant Manipulant) 샴페인을 즐길 수 있는데, 샴페인이 단순한 파티 드링크가 아닌 각각의 스토리와 맛의 개성을 갖춘 최고급 음료라는 것을 깨닫게 한다. 야경과 음악, 그리고 샴페인까지. 삼박자가 완벽하게 갖춰진 바 81은 대한민국 최고의 프러포즈 명소이자, 한국을 찾은 해외 오피니언 리더들에게도 인기 있는 방문 코스 중 하나로 자리잡고 있다.`
        }
    }
}
</script>

<style lang="scss">

</style>


