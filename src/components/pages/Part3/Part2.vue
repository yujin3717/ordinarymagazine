<template>
    <div :id="pagenum" class="page-common swiper-slide" :data-brand-name="databrandNm" data-brand-url="">
        <div class="page-common-inner" data-scrollbar>

            <div class="page-article">
                <div class="page-article">
                    <div class="spacer" style="height: 70px;"></div>

                    <div class="text-block" v-html="content">
                    </div>
                    <div class="spacer" style="height: 70px;"></div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data(){
        return{
            pagenum : 'page-9',
            databrandNm: '규정하지 않는 음악',
            content: `블루노트라는 확실한 지원군을 얻은 그는 본격적인 창작 활동을 이어갔다. 데뷔 앨범부터 세 번째 앨범 &lt;Black Stars&gt;까지 그의 오랜 동료, 그렉 오스비가 프로듀싱을 맡았다. 다음 앨범인  &lt;Modernistic&gt;부터는 제이슨 모란이 직접 프로듀싱했으며, 처음으로 밴드가 아닌 솔로로 앨범을 녹음했다. 여기에서 그는 피아노에 의지해 자작곡들을 재즈(&lt;Body And Soul&gt;), 힙합(&lt;Planet Rock&gt;), 클래식(&lt;Auf Einer Burg&gt;) 곡과 엮어 하나의 흐름으로 만들어냈다. 다양한 방면의 곡들을 하나의 호흡으로 모아내며 그는 프로듀서로의 역량을 성공적으로 증명해냈다.<br>
                        <br>
                        이후 작품들에선 특기할 지점이 자주 돌출됐다. 2006년에 발표한 앨범 &lt;Artist In Resident&gt;는 워커아트센터, 디아예술재단, 재즈앳링컨센터에서 선보였던 프로젝트에서 영감을 받았다. 힙합 트랙 &lt;Break Down&gt;, 그의 아내이자 메조소프라노 성악가인 앨리샤 홀 모란Alicia Hall Moran과 합작한 &lt;Milestone&gt;, 내레이션에 맞춰 피아노를 연주한 &lt;Artists Ought To Be Writing&gt; 등이 수록된 이 앨범은 단순한 재즈 연주자를 넘어 종합 예술가로서의 정체성을 확립한 모습을 보여준다.<br>
                        그렇다고 해서 그가 실험적인 현대 예술의 세계로 떠나가 버렸는가 하면, 그건 절대 아니다. 2010년 앨범 &lt;Ten&gt;에서는 피아노 트리오 편성을 기초로 한 정석적인 재즈 사운드를 구현한다. 이즈음부터 그는 20세기 초중반에 활동한 패츠 월러Fats Waller라는 피아니스트의 음악을 탐구했다. 고전적인 흑인 피아노 연주 장르인 래그타임Ragtime을 연주했던 인물이다. 혁신가의 이미지가 강했던 제이슨 모란이 이런 고전 아티스트에 집중한 것이 다소 의아할 수도 있겠다. 하지만 그의 디스코그래피로 돌아가 보면, 그가 2005년에 블루스를 탐구한 앨범 &lt;Same Mother&gt;를 발표했단 사실을 확인할 수 있다. 그의 혁신성과 진취성은 전통을 기반으로 한다.<br>
                        이 앨범이 패츠 월러라는 수십 년 전의 아티스트와 그의 음악을 기반으로 하고 있는 것은 사실이지만, 음악은 대단히 현대적이다. 일렉트릭 악기와 현대적인 보컬, 편곡을 더해 시대적 거리감은 전혀 느껴지지 않는다. 그의 ‘패츠 월러 프로젝트’가 더욱 주목을 받았던 것은 거대한 탈 때문이었다. 제이슨 모란은 중절모를 쓰고 담배를 물고 있는 모양의 거대한 탈을 착용한 채 피아노를 연주했는데, 이 얼굴의 주인이 바로 패츠 월러였던 것이다. 현대 아티스트가 과거 아티스트에 대한 헌정 앨범을 발표하는 것은 흔한 일이고, 그렇기에 이슈화되기는 쉽지 않다. 하지만 제이슨 모란은 이러한 시각적 효과를 더해 재즈 팬들이 주목하게 했다. 일찍이 시각예술의 힘을 알았기 때문에 가능한 프로젝트였다.`,
        }
    }
}
</script>

<style lang="scss">

</style>


