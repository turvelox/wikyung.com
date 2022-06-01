<template>

<HeaderTop />
<HeaderMain />
<ConMain />
<FooterMain />

</template>

<script>
import HeaderTop from './components/HeaderTop.vue';
import HeaderMain from './components/HeaderMain.vue';
import ConMain from './components/ConMain.vue';
import FooterMain from './components/FooterMain.vue';

export default {
  name: 'App',
  components: {
    HeaderTop,
    HeaderMain,
    ConMain,
    FooterMain
}
}
</script>

<style>
@import url("./assets/css/basic/reset.css");
@import url("./assets/css/basic/common.css");
@import url("./assets/css/basic/header.css");
@import url("./assets/css/basic/footer.css");
</style>
