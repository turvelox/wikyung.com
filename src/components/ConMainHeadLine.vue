<template>

    <div class="headline" id="headline">
        <carousel :items-to-show="1" class="headline-slider" :pause-autoplay-on-hover="false" :autoplay="2000" :wrap-around="true" >
            <slide v-for="(slide, index) in headLineItem.length" :key="index">
                <div class="headline-item" v-bind:style="headLineItem[index].bg">
                    <p class="headline-dark"></p>
                    <span class="headline-tag">{{headLineItem[index].tag}}</span>
                    <div class="headline-title">
                        <p class="headline-title-main">{{headLineItem[index].main}}</p>
                        <p class="headline-title-sub">{{headLineItem[index].sub}}</p>
                    </div>
                </div>
            </slide>
        </carousel>
        <div class="headline-back">
            <span class="headline-back-box01"></span>
            <span class="headline-back-box02"></span>
        </div>
    </div>

</template>

<script>
import 'vue3-carousel/dist/carousel.css';
import { Carousel, Slide } from 'vue3-carousel';

export default {
    name: 'ConMainHeadLine',
    components: {
        Carousel,
        Slide,
    },
    data(){
        return{
            headLineItem: [
                {
                    bg: {
                        'background-image': 'url(static/main/headline01.png)',
                    },
                    tag: "단독",
                    main: "청년취업 살피러 경제단체 중 첫 방문지로 무협 선택",
                    sub: "청년 무역인 200명 참석하는 GTEP 수료식 참석 예정"
                },
                {
                    bg: {
                        'background-image': 'url(static/main/headline02.jpg)',
                    },
                    tag: "HOT ISSUE",
                    main: "윤석열 20대 대통령 임기시작… 0시 용산벙커서 통수권 인수",
                    sub: "윤석열 대통령은 10일 0시를 기해 제20대 대통령 임기를 시작했다."
                },
                {
                    bg: {
                        'background-image': 'url(static/main/headline03.jpg)',
                    },
                    tag: "HOT ISSUE",
                    main: "뉴욕에서 '회계부정'퇴출당한 루이싱커피, 홍콩상장 추진",
                    sub: "정부 무책임한 개혁 남발"
                }
            ]
        };
    },
}
</script>

<style>

</style>