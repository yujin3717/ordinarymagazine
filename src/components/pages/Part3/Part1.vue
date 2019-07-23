<template>
    <div :id="pagenum" class="page-common swiper-slide" :data-brand-name="databrandNm" data-brand-url="">
        <div class="page-common-inner" data-scrollbar>

            <div class="page-article">
                <div class="spacer" style="height: 40px;"></div>
                <!-- full-image-block -->
                <div class="full-image-block">
                    <img class="swiper-lazy" :data-src="titelImg" alt="" src="">
                </div>
                <div class="spacer" style="height: 30px;"></div>

                <!-- text-block -->
                <div class="text-block" style="font-size: 15px; font-weight: 700; color: #343434; line-height: 26px;" v-html="content">
                </div>
                <div class="spacer" style="height: 30px;"></div>

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
            pagenum : 'page-8',
            databrandNm: '규정하지 않는 음악',
            titelImg: 'http://d2bdkorgfosgj9.cloudfront.net/ordinary/vol.27/images/pages/p05/01.jpg',
            content: `비범한 예술가는 규범과 한계를 종종 허무하게 무너뜨린다.<br>
                    제이슨 모란은 정통과 실험 사이를 자유롭게 오가며 재즈의 지평을 넓힌다.`,
            content2: `제이슨 모란Jason Moran을 향한 재즈 마니아들의 규정은 꽤 확고했다. 활동 초기, 그는 프리 재즈, 아방가르드 재즈 혹은 그보다는 난해함이 덜한 포스트 밥Post-Bop의 영역에 있는 아티스트였다. 프리 재즈의 거장인 재키 바이어드Jaki Byard, 앤드류 힐Andrew Hill, 무할 리처드 애브럼스Muhal Richard Abrams가 그의 스승이고, 그를 프로의 세계로 인도한 사람은 아방가르드 재즈 색소포니스트 그렉 오스비Greg Osby였다. 아니, 그렉 오스비는 자신의 음악을 규정하지 않았다. 재즈는 ‘자유의 음악’이지만 사실 그 안엔 화성, 박자 등 지켜야 할 요건들이 존재하며, 재즈에서의 자유란 그것들을 지키는 선에서 개성과 능력을 보여주는 데 초점이 맞춰진다. 한편, 그렉 오스비가 추구한 음악은 그러한 속박을 전부 떨쳐버리는 것이었다. 심지어는 그것을 규정하는 장르명마저도. 음악은 난해해지기 일쑤였다. 그래서 듣기 어렵거나(아방가르드), 무한히 자유로워질(프리) 수밖에 없었다. 제이슨 모란은 그런 그렉 오스비와 합을 맞추는 연주자였으니, 재즈 마니아들이 그를 그렇게 규정한 것은 당연했다.<br>
                    당시 그렉 오스비의 소속사는 재즈의 상징이자, 역사를 대변하는 음반사인 블루노트 레코드Blue Note Records였다. 그렉 오스비 밴드에서 활약하는 그의 모습은 금세 눈에 띄었다. 블루노트는 전통을 중시하는 음반사이기도 했지만, 한편으론 파격과 혁신을 통해 재즈의 진화를 이끄는 음반사이기도 했다. 블루노트는 제이슨 모란을 어떤 피아니스트로 봤을까? 프리 재즈, 혹은 정통 재즈를 대변하는 존재? 혹은 진취적인 혁신가? 분명한 사실은 제이슨 모란이 누구보다도 창의적이고 넓은 스펙트럼으로 예술 세계를 확장해가는 것을 지켜봤다는 것이다.<br>
                    <br>
                    1999년, 제이슨 모란이 발표한 데뷔 앨범 &lt;Soundtrack To Human Motion&gt;은 감상자에게 친절한 앨범은 아니었다. 멜로디가 잘 드러나지 않고, 어떠한 분위기나 감정을 환기하는 듯한 설정이 존재했다. 그는 이 앨범이 ‘한 개인이 특정한 날, 행동한 모든 것에 대한 사운드트랙’이라 정의했다. 인간이 하루에 느끼는 감정이 일관되지 않듯, 이 앨범에 실린 파편적인 느낌의 곡들은 역설적으로 하나의 흐름을 만들어냈다. 대다수의 젊은 연주자가 데뷔 앨범에서 많은 것을 보여주고 연주력이나 작곡력을 증명하려 한다면, 제이슨 모란은 이미 그 수준을 넘어선 모습을 보여줬다. 연주자이자 기획자로서의 면모를 갖췄던 것이다.`
        }
    }
}
</script>

<style lang="scss">

</style>


