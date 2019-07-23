<template>
    <div :id="pagenum" class="page-common swiper-slide" :data-brand-name="databrandNm" data-brand-url="">
        <div class="page-common-inner" data-scrollbar>

            <div class="page-article">
                <!-- full-image-block -->
                <div class="full-image-block">
                    <img class="swiper-lazy" :data-src="contentImg" alt="">
                </div>
                <div class="spacer" style="height: 20px;"></div>

                <!-- text-block -->
                <div class="text-block" v-html="content">
                </div>
                <div class="spacer" style="height: 30px;"></div>

                <!-- full-image-block -->
                <div class="full-image-block">
                    <img class="swiper-lazy" :data-src="contentImg2" alt="">
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
            pagenum : 'page-15',
            databrandNm: '음악 맛집',
            contentImg: 'https://d2bdkorgfosgj9.cloudfront.net/ordinary/vol.27/images/pages/p06/c04.jpg',
            contentImg2: 'https://d2bdkorgfosgj9.cloudfront.net/ordinary/vol.27/images/pages/p06/c05.jpg',
            content: `<strong>먼스 스컬프쳐</strong><br>
                    갤러리 카페, 먼스 스컬프쳐는 햇살 가득한 성산동의 조용한 주택가에 위치한다. 차분하면서도 느긋하게 시간의 흐름을 만끽할 수 있는 이 공간은 처음에 함미나 작가의 아틀리에 겸 카페로 시작했다. 곳곳에 놓인 책과 캔버스, 메모지를 찢어 붙인 듯 러프한 느낌의 작품들은 낯설음 속에서도 포근하고도 아늑한 온기가 느껴진다. 먼스 스컬프쳐만의 독특함은 매장 한쪽에 놓인 테크닉스 턴테이블과 함께 수많은 LP, CD, 그리고 카세트테이프에서도 발견된다. 아날로그 특유의 따뜻한 사운드가 더욱 돋보이는 로우파이, 어쿠스틱, 재즈와 같은 음악들을 계절과 날씨, 당일에 서빙하고 싶은 커피 메뉴에 맞춰 주인장이 직접 선곡한다. 그가 추천하는 재즈 앨범은 1957년에 발매된 커티스 풀러Curtis Fuller의 <The Opener>. 그가 함미나 작가로부터 처음으로 선물받은 앨범이자 앨범명처럼 LP를 수집하게 된 계기가 된 이 앨범은 잔잔하고 아름다운 트럼본 연주가 일품이다. 가장 인기가 많은 메뉴는 바닐라 라떼와 핸드메이드 파베 초콜릿. 특히 이곳의 바닐라 라떼는 시럽을 직접 만들기에 보다 달콤하고 진한 풍미가 담겨 있다. 추적추적 빗방울이 떨어지는 날이면 예민한 감성을 가진 사람들이 먼스 스컬프쳐만의 편안함과 서정적인 분위기를 찾고자 문을 두드린다.`,
        }
    }
}
</script>

<style lang="scss">

</style>


