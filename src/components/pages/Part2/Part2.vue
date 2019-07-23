<template>
    <div :id="pagenum" class="page-common swiper-slide" :data-brand-name="databrandNm" data-brand-url="">
        <div class="page-common-inner" data-scrollbar>

            <div class="page-article">
                <!-- full-image-block -->
                <div class="full-image-block">
                    <img class="swiper-lazy" :data-src="titleImg" alt="" src="">
                </div>
                <div class="spacer" style="height: 20px;"></div>

                <!-- text-block -->
                <div class="text-block" v-html="content">
                </div>
                <div class="spacer" style="height: 20px;"></div>

                <!-- youtube -->
                <div class="youtube-block">
                    <iframe draggable="false" :src="movieSrc" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"></iframe>
                </div>
                <div class="spacer" style="height: 30px;"></div>
            </div>

            <div class="page-article">
                <!-- full-image-block -->
                <div class="full-image-block">
                    <img class="swiper-lazy" :data-src="titleImg2" alt="" src="">
                </div>
                <!-- full-image-block -->
                <div class="full-image-block">
                    <img class="swiper-lazy" :data-src="titleImg3" alt="" src="">
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
            pagenum : 'page-6',
            databrandNm: '그날의 함성',
            titleImg: 'http://d2bdkorgfosgj9.cloudfront.net/ordinary/vol.27/images/pages/p04/7-8@2x.jpg',
            content: `<strong>1993, 슈퍼볼 하프타임 쇼, 로즈볼경기장</strong><br>
                    세기의 무대는 의외인 곳에서 탄생하기도 한다. 지금은 워낙 유명한 ‘슈퍼볼 하프타임 쇼’는 대학교 공연 팀이 출연하는 의례적인 프로그램이었다. 하프 타임이 시작되면 시청률은 22%나 떨어졌다. 이를 고민하던 슈퍼볼 운영진은 ‘만능 치트키’를 쓰게 되었는데, 바로 마이클 잭슨이었다. 경기는 로스앤젤레스 로즈볼경기장에서 열렸다. 월드투어 때처럼 그가 무대 한가운데에서 튀어 오르는 순간, 시청률도 함께 껑충 뛰어올랐다. &lt;Jam&gt;, &lt;Billie Jean&gt;, &lt;Black or white&gt;를 부르며 무대를 종횡무진 누볐다. 마이클 잭슨의 역대 레전드 무대 중에서도 손꼽히는 무대였다. 하이라이트는 다음이다. 당시 마이클 잭슨은 인종차별과 기아 문제에 관심을 가지고 후원 재단을 설립하고, 음악을 만드는 활동을 했다. 그가 공연 도중 신호를 보내자, 로즈볼을 메운 관중들이 파도타기를 하면서 플래카드를 들었다. 그러자 아이들이 손을 잡고 있는 그림이 ‘플래시 몹’처럼 생겨났다. 그 순간, 실제로 아이들이 무대로 들어오기 시작했다. 그렇게 마이클 잭슨은 3,500명의 합창단과 함께 &lt;Heal the World&gt;를 불렀다. 무대 퍼포먼스 역사상 가장 압도적인 순간이었다. 하프타임 쇼는 큰 성공을 거뒀고 이후 크리스티나 아길레라, 에어로 스미스, 저스틴 팀버레이크, 롤링 스톤스, 더 후, 마돈나, 비욘세, 브루노 마스 등 당대 최고의 아티스트들만 설 수 있는 최고의 무대가 되었다.`,
            titleImg2: 'http://d2bdkorgfosgj9.cloudfront.net/ordinary/vol.27/images/pages/p04/11-12@2x.jpg',
            titleImg3: 'http://d2bdkorgfosgj9.cloudfront.net/ordinary/vol.27/images/pages/p04/9_B_up@2x.jpg',
            content2: `<strong>1969, &lt;우드스탁&gt;, 베델 목장</strong><br>
                    여름이 되면 전국 각지에서 뮤직 페스티벌이 열린다. 그 시초 격인 &lt;우드스탁Woodstock Misuc & Art Fair&gt;은 이미 전설로 남은 공연이다. 60년대 말, 미국 전역에는 베트남 전쟁을 일으킨 기성세대에 대한 젊은 세대의 불만과 저항이 가득했다. ‘3일 동안 평화와 음악을 이야기하자’는 취지로 열린 이 행사는 그런 젊은이들의 마음을 흔들었다. 우드스탁은 음악 콘서트로 잘 알려졌지만 원래는 예술 퍼포먼스와 서커스 등을 포함한 프로그램이었다. 행사를 기획한 존 로버츠, 조엘 로젠먼, 마이클 랭, 아티 콘펠트는 행사 장소를 섭외하는 데 난항을 겪었다. 원래 열리기로 한 곳에서 주민들의 반대로 무산된 후 뉴욕 화이트 호수에서 베델 목장까지 이어지는 부근의 사용 허가를 받았다. 8월 15일이 되자, 공연장에는 40만 명이 넘는 관객이 몰려들었다. 공연장으로 가는 길부터 교통 체증이 생겨났고, 히피족은 공연장의 경계 울타리를 부숴버리고 차를 길 밖으로 밀어버리기도 했다. 비가 오자, 관객석은 진흙 바닥이 되어 더욱 아수라장이 되었다. 하지만 음악에 심취한 사람들은 개의치 않았다. 3일 간 32팀이 공연을 선보였고, 지미 헨드릭스가 이로 기타를 뜯어가며 화려하게 장식한 무대를 마지막으로 우드스탁은 막을 내렸다. 이 공연은 히피 문화의 정점으로 꼽히는 행사였지만, 아이러니하게도 그것이 마지막이었다. 히피 문화가 추구하던 자유분방함은 절제되지 않은 쾌락과 마약 등의 문제로 급격히 쇠퇴했다. 이후 25주년 기념 공연이 열렸지만, 예전의 명성을 누리지는 못했다. 수십만 명의 젊은이들이 뒹굴며 만끽하던 무대는 다시 평화로운 목장의 모습을 되찾았다. 지금은 작은 기념비만이 그날 여기에 그들이 있었음을 알려주고 있다.`,
            movieSrc: 'https://www.youtube-nocookie.com/embed/idg8TNknvDU?playsinline=1'
        }
    }
}
</script>

<style lang="scss">

</style>


