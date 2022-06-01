<template>
    <main class="main" id="main">

        <!-- Main Section01 & Main BG -->
        <section class="section section01">
            <div class="sec01-contents wd-1140">
                <!-- headline -->
                <ConMainHeadLine />
                <!-- poll -->
                <ConMainPoll />
            </div>
            <div class="bottom-shape">
                <span class="white"></span>
            </div>
        </section>

        <!-- Main Section02 -->
        <section class="section section02">
            <div class="wis-banner wd-1140">
                <ul class="wis-banner-list">
                    <li class="wis-banner-item wis-banner-item01">
                        <a href="#"><img src="static/main/wis-banner01.png" alt="한국의 메타버스 여기 다 모였다!" /></a>
                    </li>
                    <li class="wis-banner-item wis-banner-item02">
                        <a href="#"><img src="static/main/wis-banner02.png" alt="탄소발자국 지우기" /></a>
                    </li>
                    <li class="wis-banner-item wis-banner-item03">
                        <a href="#"><img src="static/main/wis-banner03.png" alt="오늘의 주식 시세" /></a>
                    </li>
                </ul>
            </div>
        </section>

        <!-- Main Section03 -->
        <section class="section section03">
            <!-- mnews01 -->
            <ConMainGlobal />
            <!-- mnews02 -->
            <ConMainPlan />
        </section>

        <!-- line -->
        <div class="con-line wd-1140">
            <span class="con-liner"></span>
        </div>

        <!-- Main Section04 -->
        <section class="section section04">
            
            <!-- suggest -->
            <ConMainSuggest />

        </section>
        
        <!-- Main Section05 -->
        <section class="section section05">
            
            <!-- minicon -->
            <MiniContents />

        </section>

        <!-- Main Section06 -->
        <section class="section section06">
            
            <!-- notice & event -->
            <NoticeEvent />

        </section>
    </main>
</template>

<script>
import ConMainHeadLine from './ConMainHeadLine.vue';
import ConMainPoll from './ConMainPoll.vue';
import ConMainGlobal from './ConMainGlobal.vue';
import ConMainPlan from './ConMainPlan.vue';
import ConMainSuggest from './ConMainSuggest.vue';
import MiniContents from './MiniContents.vue';
import NoticeEvent from './NoticeEvent.vue';

export default {
    name: 'ConMain',
    data(){
        
    },
    methods: {
        
    },
    components: {
    ConMainHeadLine,
    ConMainPoll,
    ConMainGlobal,
    ConMainPlan,
    ConMainSuggest,
    MiniContents,
    NoticeEvent
}
}
</script>

<style>
@import url("../assets/css/component/index.css");
</style>
