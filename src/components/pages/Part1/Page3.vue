<template>
    <div :id="pagenum" class="page-common swiper-slide" :data-brand-name="databrandNm" data-brand-url="">
        <div class="page-common-inner" data-scrollbar>

            <div class="page-article" :style="styleobject">
                <div class="header">
                    <div class="title">{{title}}</div>
                    <div class="description" v-html="description"></div>
                    <div class="editor" v-html="editor"></div>
                </div>
            </div>

            <div
                v-for="item in txtblk"
                :key="item.id"
                class="page-article"
            >
                <div :style="{height: item.height}"></div>
                <div class="content">{{ item.content }}</div>
                <div class="spacer" style="height: 5px;"></div>
                <div class="author">{{ item.author }}</div>
                <div v-if="item.isLast" style="height: 70px;"></div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data(){
        return{
            pagenum : 'page-3',
            databrandNm: '첫 문장들',
            styleobject:{
                backgroundImage: `url('http://d2bdkorgfosgj9.cloudfront.net/ordinary/vol.27/images/pages/p03/01.jpg')`,
                backgroundSize: 'cover',
                backgroundPosition: 'center center',
            },
            title: '반짝거리는',
            description: `살아있는 모든 것들의 온기.<br>찬란하게 빛나는 존재의 아름다움.`,
            editor: `<span>Editor</span> 백승원`,
            txtblk:[
                {
                    height: '20px',
                    content: '요즘, 꽃 핀 벚나무를 그리고 있는데, 그림 속에 시간의 흐름을 표현하기가 힘들어. 핀 꽃이 아니라 피어오는 꽃, 피어있는 꽃을 그리고 싶어. 그걸 그리자면 밑그림이 없이 바로 붓질을 해야 하는데, 그게 쉽지가 않아. 너네 아버지 돌아가셨을 때도 나는 밑그림 없는 세상을 생각했어. 꽃 핀 나무를 그리면서, 니 얼굴을 그리고 싶다고 생각했어. 꽃 핀 나무를 들여다보는 니 얼굴, 니 얼굴에 살아 있는 시간을 그리고 싶었어. 밑그림 없이 말이야.',
                    author: '– 김훈, <공터에서>'
                },
                {
                    height: '30px',
                    content: '토요일 아침이 왔다. 여름이라 온 세상이 밝고 상쾌하고 활기로 넘쳐났다. 모든 이의 가슴 속에 노래가 깃들어 있었고, 그 가슴이 젊다면 노래가 절로 입 밖으로 흘러나왔다. 어느 누구 할 것 없이 다들 환한 표정으로 용수철이 튕기듯 가볍게 발걸음을 옮겨놓았다. 개아카시아가 흐드러지게 피어 대기 가득 향긋한 꽃 냄새를 퍼뜨렸다. 저 너머에선 카디프 언덕이 온통 초록으로 뒤덮인 채 마을을 굽어보며 아스라이 펼쳐져 있었다. 그 모습이 마치 꿈을 꾸듯 몽롱하고 평화로워 절로 마음이 끌리는 행복의 나라처럼 보였다.',
                    author: '– 마크 트웨인, <톰 소여의 모험>'
                },
                {
                    height: '30px',
                    content: '그녀는 홀로 잠자코 선 채 먼바다를 바라보고 있었다. 그가 근처에 있음을, 숭배의 시선으로 자신을 바라보고 있음을 감지한 그녀는 조금도 부끄러워하거나 거들먹거리는 내색 없이 그에게로 눈을 돌려 그의 시선을 차분하게 받아들였다. (중략) 그는 갑작스레 그녀로부터 몸을 돌려 바닷가를 가로질러 걷기 시작했다. 그의 뺨은 불꽃처럼 이글거렸다. 몸은 벌겋게 달아올랐고 팔다리는 후들후들 떨렸다. 앞으로, 앞으로, 앞으로, 그는 앞을 향해 성큼성큼 걸어갔다. 모래사장을 넘어 저 멀리, 바다를 향해 미친 듯이 노래를 부르며, 그를 부르던 삶이 도래한 것을 환영하는 소리를 지르기도 하면서. 그녀의 모습은 그의 영혼 속에 영원토록 아로새겨져 어떠한 말로도 그의 황홀경이 빚어낸 거룩한 침묵을 깨뜨릴 수 없었다. 그녀가 눈길로 그를 불렀을 때 그의 영혼은 그 부름에 화답했다.',
                    author: '– 제임스 조이스, <젊은 예술가의 초상>',
                    isLast: true
                },
            ]
        }
    }
}
</script>

<style lang="scss">

</style>


