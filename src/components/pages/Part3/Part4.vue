<template>
    <div :id="pagenum" class="page-common swiper-slide" :data-brand-name="databrandNm" data-brand-url="">
        <div class="page-common-inner" data-scrollbar>

            <div class="page-article">
                <div class="spacer" style="height: 40px;"></div>

                <!-- full-image-block -->
                <div class="full-image-block">
                    <img class="swiper-lazy" :data-src="titleImg" alt="" src="">
                </div>
                <div class="spacer" style="height: 30px;"></div>

                <!-- text-block -->
                <div class="text-block" v-html="content">
                </div>
                <div class="spacer" style="height: 20px;"></div>

                <!-- youtube-block -->
                <div class="youtube-block">
                    <iframe width="560" height="315" :src="movieSrc" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"></iframe>
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
            pagenum : 'page-11',
            databrandNm: '규정하지 않는 음악',
            titleImg: 'http://ordinary.dev.tebah.media/vol.27/images/pages/p05/02.jpg',
            content: `우리는 ‘보여주기’의 힘이 강한 시대를 살고 있다. 시각적인 도구가 직관성이 강하다는 것을 그는 경험으로 안다. 제이슨 모란은 에이드리언 파이퍼Adrian Piper, 존 조나스Joan Jonas, 스탠 더글라스Stan Douglas 등의 미술가와 함께 작업해왔다. 또 미니애폴리스에 위치한 워커아트센터와의 오랜 합작을 통해 시각예술가로서의 면모를 키워왔다. 미술가의 무대에 즉흥 연주를 더해 ‘복제 불가능한’ 순간을 연출해내며 독보적인 시공간을 연출해내곤 했다. 반대로 자신의 연주 무대에 시각적 효과를 더하기도 했다.`,
            content2: `그는 작년에 워커아트센터에서 첫 단독 전시회를 개최했다. 전시는 대단히 성공적이어서, 이후 보스턴의 인스티튜트오브컨템포러리 아트와 웩스너센터에서도 열렸다. 올해 9월부터는 휘트니뮤지엄에서 전시한다. 제이슨 모란의 고향인 뉴욕에서 개인전이 열린다는 사실은 대단히 의미가 크다. 전시에는 다수의 재즈 연주자가 참여하며, 예술적 동지들과 협업한 새로운 작업이 공개된다. 이전과는 비교할 수 없을 정도로 큰 규모로 진행될 예정이다. 그랜드 피날레라 할 만하다.<br>
                    전시는 재즈에 대한 제이슨 모란의 갈망을 드러내기도 한다. 그는 음반이나 오래된 사진을 통해 재즈의 흔적을 찾는 것을 좋아한다. 이번 전시에서는 우리가 사진에서 가볍게 보고 흘려보내거나 놓쳤을 것들을 현실로 소환한다. 가령, 1930년대부터 1950년대까지 재즈의 중심지였던 맨해튼 52번가에 위치했던 재즈 클럽 쓰리 듀시스The Three Deuces의 방음 처리된 벽처럼. 혹은 할렘의 무도회장이었던 사보이 볼룸Savoy Ballroom의 무대 뒤 곡선형 아치에서 그는 현장의 순간을 상상한다. 아치를 따라 연주자의 음악이 무대로 뻗어 나가고, 반대로 그 아치를 따라 관객들의 소리가 무대로 쏟아지는 듯 말이다. 60~70년대의 중요한 재즈 클럽이었던 슬러그스 살룬Slug’s Saloon은 바닥에 깔린 톱밥으로 유명했는데, 그는 ‘어느 재즈 클럽도 바닥에 톱밥을 깔진 않는다’며 그것이 그 공간을 상징하는 대상이라 말한다. 단순한 이야깃거리에서 끝날 일을 그는 실제 무대를 재현해 톱밥을 깖으로써 그 시공간의 분위기를 다시 구현한다. 그리고 그 장소에 있었다는 주크박스를 설치한다. 제이슨 모란은 그러한 장치, 혹은 형태들이 단순히 시대의 모습이 아니라, 우리가 사유해야 할 역사를 담은 대상으로 본다. 소리가 나지 않는 사진을 바라보며 음악을 공부하고, 사진 속의 모습을 우리 앞에 꺼내놓는 이유가 여기에 있을 것이다.<br>
                    “저는 아주 훌륭한 음악가들에게 교육을 받았지만, 그들은 ‘프레임을 생각해야 한다’는 걸 가르쳐주지 않았어요. 빌리지 뱅가드Village Vanguard 재즈 클럽의 무대에 올라가는 것 그 자체도 프레임이에요. 그리고 그 프레임은 역사를 지니게 되죠.”`,
            movieSrc: 'https://www.youtube-nocookie.com/embed/aJ7uME3LbGc?playsinline=1'
        }
    }
}
</script>

<style lang="scss">

</style>


