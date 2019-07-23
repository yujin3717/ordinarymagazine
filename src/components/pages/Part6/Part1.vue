<template>
    <div :id="pagenum" class="page-common swiper-slide" :data-brand-name="databrandNm" data-brand-url="">
        <div class="page-common-inner" data-scrollbar>

            <div class="page-article">
                <!-- full-image-block -->
                <div class="full-image-block">
                    <img class="swiper-lazy" :data-src="titelImg" alt="" src="">
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
                <!-- text-block -->
                <div class="text-block" v-html="content2">
                </div>
                <div class="spacer" style="height: 5px;"></div>

                <!-- text-block -->
                <div class="text-block" style=" text-align: right;" v-html="content3">
                </div>
                <div class="spacer" style="height: 30px;"></div>

                <!-- text-block -->
                <div class="text-block" v-html="content4">
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
            pagenum : 'page-25',
            databrandNm: '하루키와 맥주',
            titelImg: 'https://d2bdkorgfosgj9.cloudfront.net/ordinary/vol.27/images/pages/p08/01.jpg',
            titletxt: `좋아하는 것들을 나열하면 그 사람이 보인다.<br>
                    하루키를 읽다 보면 시린 맥주 한 모금이 간절해진다.`,
            content: `노곤한 하루를 보낸 날이면 특히 간절해지는 것이 있다. 집에 오자마자 냉장고 깊숙이 넣어 둔 캔맥주를 꺼낸다. 맥주 거품이 적당하게 따른 뒤 단숨에 벌컥벌컥. 맥주의 탄산이 목구멍을 타고 흐르면 눅눅해졌던 몸과 마음이 쨍해진다. 이럴 때면 일상 최고의 보상은 오로지 차가운 맥주라는 생각까지 든다. 소설가 무라카미 하루키는 맥주에 좀 더 각별하다. 팬이라면 익히 알겠지만 그는 소문난 맥주 애호가다. 일과의 끝에, 고된 달리기 후, 여행가는 기차 식당칸 안에서 맥주를 홀짝이며 그는 ‘소확행’을 느낀다. 소확행은 ‘소소하지만 확실한 행복’, 요즘 유행하는 말이지만 1986년 하루키가 &lt;랑게르한스 섬의 오후&gt;에서 처음 쓴 말이다. 소설 속 주인공들도 자신과 닮아서 어디서든 맥주를 달고 산다. &lt;세계의 끝과 하드보일드 원더랜드&gt;의 주인공은 새벽에 일어나자마자 맥주를 들이켜고 공원에 들러 연인과 캔맥주 여섯 개를 모두 비우고도 계속 맥주 타령을 한다. &lt;1Q84&gt;의 덴고는 늘 단골 술집에서 칼스버그를 주문한다. &lt;하루키를 읽다가 술집으로&gt;의 저자는 &lt;바람의 노래를 들어라>에서 맥주 마시는 장면이 무려 56번이나 등장한다고 말한다. 하루키 스스로도 ‘맥주의 나라’에 간다면 VIP 대우를 받을 것이라고 인정한다. 물론 위스키도 좋아한다. 젊었을 때는 도쿄에서 재즈 바를 운영하며 저녁에 칵테일을 제조하기도 했다. 그래도 일상의 친구는 맥주다. “42km를 완주한 뒤에 꿀꺽꿀꺽 단숨에 마시는 맥주의 맛은 최고의 행복”이니까.`,
            content2: `<strong>개인의 취향</strong><br>
                    하루가 저물 무렵에 마시는 아주 차가운 맥주 한 병은 정말 기가 막힙니다. 이 세상에는 지나치게 차가운 맥주는 맛이 없다고 하는 까다로운 사람도 있습니다만, 나는 그렇게 생각하지 않습니다. 첫 병째 맥주는 맛을 잘 알 수 없을 정도로 아주 차가운 것이 좋습니다. 두 번째부터는 분명히 적당하게 찬 것이 맛이 있지요. 그러나 맨 처음의 맥주가 얼음처럼 차가워야 한다는 건 나의 취향입니다.`,
            content3: `-<태엽 감는 새> 중에서`,
            content4: `하루키는 맥주를 아주 차갑게 마셔야 한다고 고집한다. 물론 맥주 전문가들의 의견은 조금 다르다. 라거는 4도, 밀 맥주는 10도 내외에서 마셔야 본연의 맛을 잘 느낄 수 있다. 의외로 미지근한 정도의 온도가 맥주를 맛보기 좋은 온도다. 하지만 얼음 잔에 담겨 나오는 ‘호프식 생맥주’가 익숙한 사람에게 머리가 띵할 만큼 시원한 맥주는 여름 밤의 진리와도 같은 것이다. 하루키도 나만 맛있으면 괜찮다는 생각이다. 그리스의 한 카페에서 관자놀이가 아플 정도로 차가운 맥주를 마시고는 ‘마치 인생의 양지와 같은 하루’라고 기록할 정도니까.`
        }
    }
}
</script>

<style lang="scss">

</style>


