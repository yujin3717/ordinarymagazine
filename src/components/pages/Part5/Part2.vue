<template>
    <div :id="pagenum" class="page-common swiper-slide" :data-brand-name="databrandNm" data-brand-url="">
        <div class="page-common-inner" data-scrollbar>

            <div class="page-article">
                <div class="spacer" style="height: 70px;"></div>

                <!-- text-block -->
                <div class="text-block" v-html="content">
                </div>
                <div class="spacer" style="height: 20px;"></div>

                <!-- full-image-block -->
                <div class="full-image-block">
                    <img class="swiper-lazy" :data-src="contentImg" alt="" src="">
                </div>
                <!-- full-image-block -->
                <div class="full-image-block">
                    <img class="swiper-lazy" :data-src="contentImg2" alt="" src="">
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
            pagenum : 'page-18',
            databrandNm: 'Every is a New Beginning',
            contentImg: 'http://d2bdkorgfosgj9.cloudfront.net/ordinary/vol.27/images/pages/p07/content-2/01.png',
            contentImg2: 'http://d2bdkorgfosgj9.cloudfront.net/ordinary/vol.27/images/pages/p07/content-2/02.png',
            content: `<strong>바이어드 레인의 작은 숍</strong><br>
                    영국의 대표적인 디자이너이자 기사 작위를 보유한 폴 스미스는 자신의 이름을 딴 패션 브랜드를 50여 년간 최정상에서 이끌고 있다. 전 세계 73개국에 매장을 운영하며 지금까지도 모든 디렉팅을 직접 한다. 결코 쉽지 않은 행보다. 그 시작은 작은 단칸방이었다. 폴 스미스는 1970년 영국 북부인 노팅엄 6 바이야드 레인에 쇼룸을 오픈했다. 가로와 세로가 약 3m 되는 좁은 방이었지만 그래도 매장이라고 불렀다. 매장은 금요일과 토요일에만 문을 열었고 생계를 유지하기 위해 택시를 몰거나 아르바이트를 해야 했다. 힘이 되어 준 건 지금의 아내인 폴린이었다. 그에게 옷을 만드는 법을 알려준 것도, 매장을 내라고 용기를 준 것도 그였다. 매장은 3년 뒤, 10 바이야드 레인으로 이전하면서 정규적으로 운영하는 공간으로 성장했다. 1976년 폴 스미스는 파리 컬렉션에서 첫 쇼를 선보이게 된다. 한 호텔의 객실이었다. “나의 첫 컬렉션은 셔츠 6벌, 점퍼 2벌, 수트 2벌로 구성했으며 검은색 펠트 천을 덮은 침대 위에 옷을 펼쳐 놓았다. 쇼 마지막 날 딱 한 명의 손님이 찾아왔다. 그 사람이 주문하면서 나의 사업이 시작되었다.”<br>
                    전시장에는 첫 매장의 크기를 그대로 재현한 공간이 있다. 몇 걸음도 안 되는 작디작은 공간이다. 화려한 볼거리가 많은 전시임에도 공간이 가장 기억에 남는 것은 왜일까. 다음 세대의 디자이너들에게 가장 하고 싶은 메시지가 이곳에 압축되어 있다.`,
            content2: `<strong>일상에서 얻는 영감</strong><br>
                    폴 스미스의 손에 늘 들려 있는 것이 있다. 카메라 혹은 아이폰. 어디를 가든 흥미로운 것이 나타나면 그는 재빨리 카메라를 꺼낸다. 온 세상의 재미있는 것은 모두 내 것으로 저장하려는 듯이. 아마추어 사진가였던 아버지의 영향을 받아 특히 애착을 가진 것을 그도 인정한다. 또한 익히 알려진 대로 그는 엄청난 수집광이다. 런던 코벤트 가든에 위치한 그의 사무실 벽에는 빈틈 하나 없을 만큼 액자가 빽빽하다. 수집품은 전시장에도 걸려있다. 수백 개의 액자는 그의 사무실처럼 세 개의 너른 벽면을 거뜬히 메운다. 앤디 워홀, 데이비드 호크니처럼 값비싼 작가의 작품도 있고 직접 찍은 사진이나 일러스트, 포스터 등 각양각색이다. 책상 위에는 겹겹이 쌓은 책, 기념품, 팬들의 선물 등으로 가득해서 원래 용도로는 도저히 쓸 수 없을 정도다. ‘일상 어디에서든 영감을 받을 수 있다’는 모토를 자신이 매일 실천하는 셈이다. 많은 물건 중에서도 눈에 띄었던 것은 우표가 덕지덕지 붙은 오브제들이다. 1998년부터 익명의 팬이 보내온다는 ‘묻지마’식 선물이다. 볼링 핀, 장난감 차, E.T 인형 심지어 화장실 청소용 솔도 있다.`
        }
    }
}
</script>

<style lang="scss">

</style>


