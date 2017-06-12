<template>
    <div>
        <v-pc-page v-if="isPC"></v-pc-page>
        <v-phone-page v-else></v-phone-page>
    </div>
</template>

<style scoped>
</style>

<script type="text/javascript">
    import pcPage from '../pcPage/pcPage.vue';
    import phonePage from '../phonePage/phonePage.vue';

    export default {
        components: {
            'v-pc-page': pcPage,
            'v-phone-page': phonePage
        },
        data() {
            return {
                isPC: true
            }
        },
        created() {
            let sUserAgent = navigator.userAgent.toLowerCase();
            console.log(sUserAgent);
            let bIsIpad = sUserAgent.match(/ipad/i) == "ipad";
            let bIsIphoneOs = sUserAgent.match(/iphone os/i) == "iphone os";
            let bIsMidp = sUserAgent.match(/midp/i) == "midp";
            let bIsUc7 = sUserAgent.match(/rv:1.2.3.4/i) == "rv:1.2.3.4";
            let bIsUc = sUserAgent.match(/ucweb/i) == "ucweb";
            let bIsAndroid = sUserAgent.match(/android/i) == "android";
            let bIsCE = sUserAgent.match(/windows ce/i) == "windows ce";
            let bIsWM = sUserAgent.match(/windows mobile/i) == "windows mobile";
            if (bIsIpad || bIsIphoneOs || bIsMidp || bIsUc7 || bIsUc || bIsAndroid || bIsCE || bIsWM) {
                console.log("Phone");
                this.isPC = false;
            } else {
                console.log("PC");
                this.isPC = true;
            }
        }
    }
</script>