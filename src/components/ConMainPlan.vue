<template>

    <div class="mnews wd-1140">
        <div class="mnews-tag">
            <img class="mnews-tag-icon" src="static/common/gnb_icon_07.png" alt="-" />
            <span class="mnews-tag-text">기획/탐사</span>
            <span class="mnews-tag-line"></span>
        </div>
        <carousel :items-to-show="3" :pause-autoplay-on-hover="false" :autoplay="3000" :wrap-around="true" class="mnews-list shortnews">
            <slide v-for="(slide, index) in planItem.length" :key="index">
                <div class="mnews-item mnews-item01">
                    <div class="mnews-item-thum">
                        <a href="#"><span class="mnews-item-thum-img" v-bind:style="planItem[index].thum"></span></a>
                    </div>
                    <div class="mnews-item-copy">
                        <ul class="mnews-item-copy-info">
                            <li class="mnews-item-copy-info-image" v-bind:style="planItem[index].userImg"></li>
                            <li class="mnews-item-copy-info-name">{{planItem[index].userName}}</li>
                            <li class="mnews-item-copy-info-hash">{{planItem[index].hash[0]}}</li>
                            <li class="mnews-item-copy-info-hash">{{planItem[index].hash[1]}}</li>
                        </ul>
                        <p class="mnews-item-copy-title">
                            <a href="#">{{planItem[index].title}}</a>
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
    name: 'ConMainPlan',
    components: {
        Carousel,
        Slide,
        Navigation
    },
    data(){
        return{
            planItem: [
                {
                    thum: {
                        'background-image': 'url(static/main/shortnews-thum01.png)',
                    },
                    userImg: {
                        'background-image': 'url(static/common/user-default.png)',
                    },
                    userName: "김영진 기자",
                    hash: ["#기획/탐사", "#사고력"],
                    title: "김태호PD의 콘텐츠 지향적 사고법! 그것을 파헤쳐보자!"
                },
                {
                    thum: {
                        'background-image': 'url(static/main/shortnews-thum02.png)',
                    },
                    userImg: {
                        'background-image': 'url(static/common/user-default.png)',
                    },
                    userName: "김영진 기자",
                    hash: ["#기획/탐사", "#사고력"],
                    title: "한국 스타트업에 투자한 글로벌 투자사 20곳"
                },
                {
                    thum: {
                        'background-image': 'url(static/main/shortnews-thum03.png)',
                    },
                    userImg: {
                        'background-image': 'url(static/common/user-default.png)',
                    },
                    userName: "김영진 기자",
                    hash: ["#기획/탐사", "#사고력"],
                    title: "배민-직방-야놀자-토스 자회사 운영전략으로 한층더 성장하기!"
                },
                {
                    thum: {
                        'background-image': 'url(static/main/shortnews-thum04.png)',
                    },
                    userImg: {
                        'background-image': 'url(static/common/user-default.png)',
                    },
                    userName: "김영진 기자",
                    hash: ["#기획/탐사", "#사고력"],
                    title: "성과가 나빠진 팀원을 되살리는 '피드백 기술'"
                },
                {
                    thum: {
                        'background-image': 'url(static/main/shortnews-thum05.png)',
                    },
                    userImg: {
                        'background-image': 'url(static/common/user-default.png)',
                    },
                    userName: "김영진 기자",
                    hash: ["#기획/탐사", "#사고력"],
                    title: "2021년 주요 스타트업 실적, 업종별 정리!"
                },
                {
                    thum: {
                        'background-image': 'url(static/main/shortnews-thum06.png)',
                    },
                    userImg: {
                        'background-image': 'url(static/common/user-default.png)',
                    },
                    userName: "김영진 기자",
                    hash: ["#기획/탐사", "#사고력"],
                    title: "연 10배 성장 비결부터 '아이템 표절' 논란까지.. 킥보드 업체 '스윙' 이야기"
                },
                
            ]
        };
    },
}
</script>

<style>
</style>