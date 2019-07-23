<template>
    <div :id="pagenum" class="page-common swiper-slide" :data-brand-name="databrandNm" data-brand-url="">
        <div class="page-common-inner" data-scrollbar>

            <div class="page-article">
                <!-- full-image-block -->
                <div class="full-image-block">
                    <img class="swiper-lazy" :data-src="titelImg" alt="" src="">
                </div>
                <div class="spacer" style="height: 10px;"></div>

                <!-- text-block -->
                <div class="text-block" style="font-size: 13px; color: #343434; line-height: 20px; text-align: center;" v-html="titletxt"></div>
                <div style="height: 30px;"></div>

                <!-- text-block -->
                <div class="text-block" v-html="content">                    
                </div>
                <div clas="spacer" style="height: 40px;"></div>
            </div>

            <div class="page-article">
                <!-- full-image-block -->
                <div class="full-image-block">
                    <img class="swiper-lazy" :data-src="titleImg2" alt="" src="">
                </div>
                <div class="spacer" style="height: 20px;"></div>

                <!-- text-block -->
                <div class="text-block" v-html="content2">                    
                </div>
                <div style="height: 70px;"></div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data(){
        return{
            pagenum : 'page-5',
            databrandNm: '그날의 함성',
            titelImg: 'http://d2bdkorgfosgj9.cloudfront.net/ordinary/vol.27/images/pages/p04/3@2x.jpg',
            titletxt: `긴장감과 아드레날린을 최고조로 끌어올리는 라이브 공연.<br>열기와 함성이 울려 퍼졌던 그날, 역사의 무대들`,
            content: `<strong>1985, &lt;라이브 에이드&gt;, 웸블리스타디움 & 존 F. 케네디스타디움</strong><br>
                    1985년 아프리카 기아 난민의 후원 모금을 모으기 위해 공연된 &lt;라이브 에이드Live Aid&gt;는 150여 개국에서 약 19억 명의 시청자가 동시에 방송을 본, 역사상 대규모의 실시간 위성 중계 방송으로 꼽힌다. 공연은 런던 웸블리스타디움과 존 F. 케네디스타디움에서 동시에 진행되었으며 영국은 BC, 미국은 ABC에서 방송을 송출했다(시차 때문에 실제로는 영국에서 먼저 시작되었다). 데이비드 보위, 엘튼 존, 에릭 클랩튼, 믹 재거, 밥 딜런, 롤링 스톤스, 스팅, U2, 퀸, 레드 제플린, 듀란듀란, 마돈나 등 믿기 힘든 초호화 캐스팅이었다. 공연에는 영국 22팀, 미국 35팀이 참여했으며 팀마다 약 20분의 공연 시간이 주어졌는데 무려 16시간의 러닝 타임으로 진행되었다. 웸블리스타디움에는 약 7만 명이, 존 F. 케네디스타디움에는 약 9만 명의 관중이 몰려들었다. 얼마 전 화제가 되었던 영화 &lt;보헤미안 랩소디&gt;에 묘사된 것처럼 퀸은 전설적인 라이브 무대를 선보였고 두고두고 회자되는 장면들이 탄생했다. 특히 제네시스의 드러머, 필 콜린스는 영국에서 공연한 뒤 바로 미국으로 건너가 공연에 합류해 ‘대륙 간 퍼포먼스’를 완성했다. &lt;라이브 에이드&gt;는 전 세계의 약 40%나 되는 사람들이 동시에 지켜본, 앞으로 다시 없을 실시간 공연이었다.`,
            titleImg2: 'http://d2bdkorgfosgj9.cloudfront.net/ordinary/vol.27/images/pages/p04/5-6@2x.jpg',
            content2: `<strong>1984, &lt;굿모닝 미스터 오웰&gt;, WNET스튜디오 & 퐁피두센터</strong><br>
                    &lt;라이브 에이드&gt;의 경우처럼 두 대륙에서 동시에 공연을 열고, 이 방송을 전 세계에 송출한다는 실험적인 아이디어를 일 년 전 먼저 시도한 사람이 있다. 백남준은 조지 오웰이 빅 브라더의 시대를 예견한 소설 &lt;1984&gt;에 맞춰 1984년 새해에 방영하는 인공위성 생방송 &lt;굿모닝 미스터 오웰&gt;을 기획했다. 뉴욕의 방송국인 WNET스튜디오와 파리의 퐁피두 센터에 스튜디오를 마련하고 실시간 연결하는 방송이었다. 지금이야 핸드폰만 있으면 라이브 방송을 볼 수 있는 시대지만, 당시에는 획기적인 발상이었다. 백남준은 오웰이 예견했던 것처럼 텔레비전이 거대한 감시자가 아니라, 소통하는 매체이며 우리는 그 시대를 잘 살아가고 있다는 메시지를 건네고 싶었다. 방송은 빨간 입술이 “굿모닝, 미스터 오웰”이라고 인사하는 장면부터 시작한다. 서로 만난 적 없는 세기의 천재 뮤지션이 인공위성을 통해 서로 연결되는 모습도 담겼다. 파리에서 요셉 보이스가 피아노를 치고 미국에 있는 존 케이지가 선인장을 연주하며 협업한 것이다. 이브 몽탕이 탭댄스를 추고 샬럿 무어먼이&lt;TV첼로&gt;를 연주하며 우주복을 입은 80명의 무용수가 퐁피두 센터에서 한바탕 퍼포먼스를 벌였다. 이 방송은 세계 최초의 국제 위성 설치 작품으로 기록됐다. 공연 도중 위성 연결이 잠시 끊어지는 일도 벌어졌지만, 백남준은 기술적인 문제가 오히려 ‘살아 있는 분위기’를 고조시켰다고 말했다. 이 방송은 미국과 독일 그리고 한국에 생방송으로 방영되었고 2,500만 명의 사람들이 지켜보았다.`
        }
    }
}
</script>

<style lang="scss">

</style>


