<template>
    <div>
        <div class="header-div">
            <img class="header-bg" src="../../assets/header_bg.png">
            <img class="header-title" src="../../assets/header_title.png">
            <img class="header-phone" src="../../assets/header_phone.png">
            <img class="header-qrcode" src="../../assets/qrcode.png">
            <img class="header-download-text" src="../../assets/header_download_text.png">
        </div>

        <div class="content-div">
            <img class="content-01" src="../../assets/content_01.png">
            <img class="content-02" src="../../assets/content_02.png">
        </div>

        <div class="footer-div">
            <img class="footer-bg" src="../../assets/footer_bg.png">
            <img class="footer-text" src="../../assets/footer_text.png">
            <img class="footer-download-text" src="../../assets/footer-download-text.png">
            <img class="footer-qrcode" src="../../assets/qrcode.png">
        </div>
    </div>
</template>

<style scoped>
    .header-div {
        position: relative;
    }

    .header-bg {
        width: 100%;
        height: auto;
    }

    .header-title {
        position: absolute;
        width: 26%;
        height: auto;
        top: 20%;
        left: 18%;
    }

    .header-qrcode {
        position: absolute;
        width: 12%;
        height: auto;
        bottom: 10%;
        left: 18%;
    }

    .header-download-text {
        position: absolute;
        width: 12%;
        height: auto;
        bottom: 10%;
        left: 32%;
    }

    .header-phone {
        position: absolute;
        width: 46%;
        height: auto;
        top: 8%;
        right: 8%;
    }

    .content-div {
        margin-top: 4%;
        text-align: center;
    }

    .content-01 {
        width: 80%;
        height: auto;
    }

    .content-02 {
        margin-top: 8%;
        width: 80%;
        height: auto;
    }

    .footer-div {
        position: relative;
        margin-top: 10%;
    }

    .footer-bg {
        width: 100%;
        height: auto;
    }

    .footer-text {
        position: absolute;
        top: 38%;
        left: 14%;
        width: 40%;
    }

    .footer-download-text {
        position: absolute;
        top: 18%;
        right: 30%;
        width: 10%;
    }

    .footer-qrcode {
        position: absolute;
        top: -70%;
        right: 16%;
        width: 12%;
    }
</style>

<script type="text/javascript">
    export default {}
</script>