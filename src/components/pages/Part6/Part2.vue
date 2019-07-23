<template>
    <div :id="pagenum" class="page-common swiper-slide" :data-brand-name="databrandNm" data-brand-url="">
        <div class="page-common-inner" data-scrollbar>

            <div class="page-article">
                <div class="spacer" style="height: 70px;"></div>
                <!-- text-block -->
                <div class="text-block" v-html="content">
                </div>
                <div class="spacer" style="height: 5px;"></div>
                <!-- text-block -->
                <div class="text-block" style=" text-align: right;" v-html="content2">
                </div>
                <div class="spacer" style="height: 30px;"></div>

                <!-- text-block -->
                <div class="text-block" v-html="content3">
                </div>
                <div class="spacer" style="height: 30px;"></div>
            </div>

            <div class="page-article">
                <!-- text-block -->
                <div class="text-block" v-html="content4">
                </div>
                <div class="spacer" style="height: 5px;"></div>
                <!-- text-block -->
                <div class="text-block" style=" text-align: right;" v-html="content5">
                </div>
                <div class="spacer" style="height: 30px;"></div>

                <!-- text-block -->
                <div class="text-block" v-html="content6">
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
            pagenum : 'page-26',
            databrandNm: '하루키와 맥주',
            titelImg: 'http://d2bdkorgfosgj9.cloudfront.net/ordinary/vol.27/images/pages/p08/01.jpg',
            titletxt: `좋아하는 것들을 나열하면 그 사람이 보인다.<br>
                    하루키를 읽다 보면 시린 맥주 한 모금이 간절해진다.`,
            content: `<strong>굴 튀김과 삿포로</strong><br>
                    나는 그것을 차분하게 입으로 가져간다. 튀김 옷과 굴이 내 입 안으로 들어간다. 바삭한 튀김 옷을 씹을 때의 감촉과 부드러운 굴을 씹을 때의 감촉이 당연히 공존해야 할 식감으로 동시에 감지된다. 미묘하게 뒤섞인 향이 축복처럼 입 안에서 퍼져간다. 나는 지금 행복하다. 나는 굴 튀김이 먹고 싶었고, 그리고 이렇게 여덟 개짜리 굴 튀김을 음미할 수 있으니까. 게다가 짬짬이 맥주까지 마실 수 있다.`,
            content2: `-<잡문집> 중 ‘자기란 무엇인가’`,
            content3: `하루키는 원고지 4매 이내로 ‘진정한 자신은 무엇인가?’라는 주제를 가지고 써야 한다면 굴 튀김에 대해 쓰는 게 낫다고 생각한다. 굴 튀김을 아주 좋아하기 때문이다. 그는 단골집에 들러 굴 튀김 8개짜리 접시와 중간 사이즈의 삿포로 병을 주문하고는 행복해한다. 갓 튀겨내, 지글지글 소리를 내는 접시 위의 굴 튀김을 바라보면서 이 순간 자신이 굴이 아니라 소설가라는 사실을 기뻐한다. 거기에 삿포로 맥주를 마신다. 자신이 직접 밝힌 맥주 1위는 삿포로 블랙 라벨. 2위는 산토리 프리미엄 몰츠다. 하이네켄도 좋아한다. 보통은 산뜻하고 깔끔한 맛의 라거를 좋아한다. 비교적 최근에는 IPA(인디아 페일 에일)에 빠졌다. “언젠가 기회가 되면 하와이에 날아가서 ‘빅스웰 IPA’를 생맥주로 마셔보고 싶다.” 진짜 맛있는 술은 여행하지 않는다. 그 술을 맛보려는 사람이 여행할 뿐.`,
            content4: `<strong>기차 식당칸과 모닝 맥주</strong><br>
                    대학에 다닐 때 방학이 되면, 나는 옷가지가 담긴 여행 가방을 들고, 아침의 첫 신칸센 열차에 올랐다. 창가의 좌석에 앉아, 책을 읽고, 풍경답지 않은 풍경을 바라보고, 햄 샌드위치를 먹고, 맥주를 마셨다. 그러한 아침에 맥주를 마신다는 것은, 나에게 있어서는 하나의 의식 같은 것이었다.`,
            content5: `-<지금은 없는 공주를 위하여> 중 ‘5월의 해안선’`,
            content6: `하루키가 기차 식당칸을 좋아하는 이유는 아침이라도 눈치 보지 않고 맥주를 마실 수 있어서다. 지나가는 풍경을 바라보면서 마시는 술 한 잔은 작은 일탈을 선사한다. 소설 <양을 쫓는 모험>,
                    <댄스 댄스 댄스>에서도 기차를 타고 가면서 이른 아침부터 맥주를 마시는 주인공들이 등장한다. 그들은 잠시 하루키의 대변인이 되어 맥주 사랑을 설파한다. <세계의 끝과 하드보일드 원더랜드>의 주인공 역시 이렇게 중얼거린다.”
                    나는 햇살이 눈부시게 쏟아지는 잔디밭에 누워서 음악을 들으며, 시원한 맥주를 마시고 싶다. 그 이상은 아무것도 바라지 않는다.” 하루키는 무더운 여름날, 짧은 반바지를 입고 로큰롤을 들으며 맥주를 마시는 시간을 최고의 시간으로 꼽는다. 올여름에는 하루키의 책에 얼굴을 묻고 그가 안내하는 대로 맥주의 시간을 보내도 괜찮을 것 같다.`

        }
    }
}
</script>

<style lang="scss">

</style>


