<template>

    <div class="mnews wd-1140">
        <div class="mnews-tag">
            <img class="mnews-tag-icon" src="static/common/gnb_icon_08.png" alt="-" />
            <span class="mnews-tag-text">글로벌르포</span>
            <span class="mnews-tag-line"></span>
        </div>
        <carousel :items-to-show="3" :pause-autoplay-on-hover="false" :autoplay="3000" :wrap-around="true" class="mnews-list coinnews">
            <slide v-for="(slide, index) in globalItem.length" :key="index">
                <div class="mnews-item mnews-item01">
                    <div class="mnews-item-thum">
                        <a href="#"><span class="mnews-item-thum-img" v-bind:style="globalItem[index].thum"></span></a>
                    </div>
                    <div class="mnews-item-copy">
                        <ul class="mnews-item-copy-info">
                            <li class="mnews-item-copy-info-image" v-bind:style="globalItem[index].userImg"></li>
                            <li class="mnews-item-copy-info-name">{{globalItem[index].userName}}</li>
                            <li class="mnews-item-copy-info-hash">{{globalItem[index].hash[0]}}</li>
                            <li class="mnews-item-copy-info-hash">{{globalItem[index].hash[1]}}</li>
                        </ul>
                        <p class="mnews-item-copy-title">
                            <a href="#">{{globalItem[index].title}}</a>
                        </p>
                    </div>
                </div>
            </slide>
            <template #addons>
                <navigation />
            </template>
        </carousel>
    </div>

</template>

<script>
import 'vue3-carousel/dist/carousel.css';
import { Carousel, Slide, Navigation } from 'vue3-carousel';

export default {
    name: 'ConMainGlobal',
    components: {
        Carousel,
        Slide,
        Navigation
    },
    data(){
        return{
            globalItem: [
                {
                    thum: {
                        'background-image': 'url(static/main/coinnews-thum01.png)',
                    },
                    userImg: {
                        'background-image': 'url(static/common/user-default.png)',
                    },
                    userName: "김영진 기자",
                    hash: ["#글로벌르포", "#이어령"],
                    title: "인재가 되고픈 이들에게, 이어령이 남긴 89년짜리 생각"
                },
                {
                    thum: {
                        'background-image': 'url(static/main/coinnews-thum02.png)',
                    },
                    userImg: {
                        'background-image': 'url(static/common/user-default.png)',
                    },
                    userName: "김영진 기자",
                    hash: ["#글로벌르포", "#포켓몬빵"],
                    title: "마케팅의 힘! 이번 포켓몬 빵의 핵심 주제는 무엇일까?"
                },
                {
                    thum: {
                        'background-image': 'url(static/main/coinnews-thum03.png)',
                    },
                    userImg: {
                        'background-image': 'url(static/common/user-default.png)',
                    },
                    userName: "김영진 기자",
                    hash: ["#글로벌르포", "#경제"],
                    title: "누구나 부자가 되고싶다. 하지만 부자가 되는 사람은 따로 있다."
                },
                {
                    thum: {
                        'background-image': 'url(static/main/coinnews-thum04.png)',
                    },
                    userImg: {
                        'background-image': 'url(static/common/user-default.png)',
                    },
                    userName: "김영진 기자",
                    hash: ["#글로벌르포", "#스타트업"],
                    title: "최초 투자 92% 매쉬업엔젤스가 스타트업 투자를 결정하는 기준"
                },
                {
                    thum: {
                        'background-image': 'url(static/main/coinnews-thum05.png)',
                    },
                    userImg: {
                        'background-image': 'url(static/common/user-default.png)',
                    },
                    userName: "김영진 기자",
                    hash: ["#글로벌르포", "#밈"],
                    title: "밈 끝판왕 '9GAG'로 보는 커뮤니티 사업의 고난과 슬픔"
                },
                {
                    thum: {
                        'background-image': 'url(static/main/coinnews-thum06.png)',
                    },
                    userImg: {
                        'background-image': 'url(static/common/user-default.png)',
                    },
                    userName: "김영진 기자",
                    hash: ["#AD", "#프로모션"],
                    title: "기업DB 장기이용권 45% 할인 프로모션을 진행합니다."
                },
                
            ]
        };
    },
}
</script>

<style>
</style>