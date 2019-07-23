<template>
    <div :id="pagenum" class="page-common swiper-slide" :data-brand-name="databrandNm" data-brand-url="">
        <div class="page-common-inner" data-scrollbar>

            <div class="page-article">
                <div class="spacer" style="height: 40px;"></div>

                <!-- video-block.fixed-horizontal -->
                <div class="video-block fixed-horizontal w16-9" @click.prevent="isClick = !isClick">
                    <div v-if="!isStart" class="overlay" :style="{display:[!isStart? 'flex' : 'none']}">
                        <div class="title" v-html="videotitle"></div>

                        <div class="play">
                            <button
                                id="play"
                                v-bind:style="{display:[paused? 'inline-block' : 'none']}"
                                @click.stop="startplay"
                                type="button"><i class="cuscon-play"></i></button>
                        </div>
                    </div>
                    <div v-if="!isStart" :style="{display:[!isStart? 'block' : 'none']}" class="poster swiper-lazy" :data-background="poster"></div>

                    <div v-if="isHidden" :style="{display:[!isClick? 'block' : 'none']}" class="control" >
                        <div class="control-inner">
                            <div class="sound">
                                <button @click.stop="muted"
                                  type="button"
                                  v-bind:class="[ismuted? 'off' : 'on']"
                                ></button>
                            </div>

                            <div class="pause">
                                <button id="pause"
                                    v-bind:style="{display:[playing? 'inline-block' : 'none']}"
                                    v-show="playing"
                                    @click.stop="pause"
                                    type="button"
                                    class="pause-btn"><i class="cuscon-ios-pause"></i></button>
                                <button id="play"
                                    v-bind:style="{display:[paused? 'inline-block' : 'none']}"
                                    v-show="paused"
                                    @click.stop="play"
                                    type="button"
                                    class="replay-btn"><i class="cuscon-play"></i></button>
                            </div>
                        </div>
                    </div>
                    <div class="video" >
                        <video v-on:ended="setEnded" id="innervideoPlayer" v-play="playing" muted="muted" playsinline="true" preload="metadata">
                            <source :src="videosrc" type="video/mp4">
                            브라우저가 Video 태그를 지원하지 않습니다.
                        </video>
                    </div>
                </div>
                <div class="spacer" style="height: 30px;"></div>

                <!-- text-block -->
                <div class="text-block" v-html="content">
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
            // 실행, 음소거, 일시정지버튼 숨김여부 토큰
            playing: false,
            ismuted: true,
            isStoped: false,
            isHidden: false,
            isEnded: false,
            isStart: false,
            ispaused: false,
            isClick: false,
            pagenum : 'page-17',
            databrandNm: 'Every is a New Beginning',
            poster: 'http://d2bdkorgfosgj9.cloudfront.net/ordinary/vol.27/video/video-poster.jpg',
            videosrc: 'http://d2bdkorgfosgj9.cloudfront.net/ordinary/vol.27/video/video.mp4',
            videotitle: '',
            content: `폴 스미스의 전시가 한국을 찾는다는 소식을 들었을 때 문득 9년 전 열렸던 전시 하나가 떠올랐다. 대림미술관의 &lt;Inside Paul Smith&gt;. 관람객 4만 명이라는 놀라운 흥행 성적을 거뒀던 전시다. 아는 사람만 찾아갔던 사진 전문 미술관에서 전시만 열렸다 하면 줄을 서서 입장하는 미술관으로 터닝포인트가 되었던 시기다. 실제로 체감한 폴 스미스의 브랜드 파워는 대단했다. 2017년 도쿄의 편집숍인 ‘라카구la kagu’에서 마련한 전시도 그랬다. 편집숍 맨 위층에는 폴 스미스가 디자인할 때 영감을 받은 책과 사진 등을 주제별로 전시하는 한편, 컬래버레이션 의상을 선보였다. 한정판이라 그랬는지 선보인 가죽 자켓은 이미 매진된 뒤였다. 이번에 열리는 전시 역시 전적이 화려하다. &lt;Hello, My name is Paul Smith&gt;는 2013년 런던 디자인뮤지엄the Design Museum에서 기획한 전시로 34만 명이라는 미술관 역사상 가장 많은 관람 수를 기록했다. 이 투어 전시가 11번째로 우리나라를 찾았다. 누구나 인정하는 최고의 패션 디자이너지만 패션에 국한된 전시였다면 지금의 인기를 구가하기 어려웠을 것이다. 디자인, 미술, 사진, 건축 등 다양한 분야를 아우르는 내용의 대부분은 그의 일상과 연관된 것들이다. 그가 좋아하는 것들로 가득 꾸린 방은 즐겁고, 유쾌하고, 신기하고, 호기심이 넘친다. 그건 폴 스미스라는 인물 그 자체다. 이번 전시는 2010년보다 좀 더 진화한 버전이다. 왜냐하면 그는 지금도 매일 새롭게 업그레이드되는 중인 것 같으니까. 전시는 그가 처음 어떻게 디자이너가 되었고 어디에서 영감을 받는지 그리고 그 원동력은 무엇인지 살핀다.`
        }
    },
    mounted(){
        const self = this;
        // 페이지 이동시 Video Pause
        this.EventBus.$on('pauseVideo', function(){
            self.playing = false;
        });
    },
    directives: {
        play: {
            bind(el, binding, vnode) {
                el.addEventListener('playing', () => {
                vnode.context[binding.expression] = !el.paused;
                });
                el.addEventListener('pause', () => {
                vnode.context[binding.expression] = !el.paused;
                });
                vnode.context[binding.expression] = !el.paused;
            },
            update(el, binding) {
                if (el.paused) {
                    if (binding.value) {
                        el.play();
                    }
                } else if (!binding.value) {
                    el.pause();
                }
            }
        }
    },
    methods:{
        play() {
            this.playing = true;
            this.isStoped = false;
        },
        pause() {
            this.playing = false;
            this.isStoped = true;
        },
        muted(){
            this.ismuted = !this.ismuted;
            document.getElementById('innervideoPlayer').muted = this.ismuted;
        },
        setVideo(){

        },
        setEnded(){
            this.playing = false;
            this.isEnded = true;
        },
        handleModal(){
            this.isEnded = false;
            this.isStoped = true;
        },
        videoDone(){
            this.isEnded = true;
        },
        startplay(){
            this.isStart = true;
            this.playing = true;
            this.isHidden = true;
            this.isClick = false;
        }
    },
    computed:{
        paused() {
            return !this.playing;
        }
    }
}
</script>

<style lang="scss">

</style>


