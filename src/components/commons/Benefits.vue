<template>
<div class="ms_benefits">
    <div class="ms_container">
        <div class="ms_text text-center">
            <div class="ms_subtitle">
                Maxcoach available courses
            </div>
            <div class="ms_title1">
                Access 
                <span class="ms_color">
                    Smart Tutoring 
                </span>
                Program For Benefits
            </div>
        </div>
        <div class="row row-cols-3">
            <div class="col ms_box">
                <div class="ms_img">
                    <img src="../../assets/img/home-2-image-box-01.png" alt="">
                </div>
                <div class="ms_title2">
                    Customize Preferences
                </div>
                <div class="ms_subtitle1">
                    Learners are given the right to arrange and customize their study schedule and timetable based on preferences.
                </div>
                <a href="#">
                    Start here &rarr;
                </a>
            </div>
            <div class="col ms_box">
                <div class="ms_img">
                    <img src="../../assets/img/about-us-02-image-box-02.png" alt="">
                </div>
                <div class="ms_title2">
                    Cloud Storage
                </div>
                <div class="ms_subtitle1">
                    You can store online lessons via online cloud or download to your device and revise lessons on the way.
                </div>
                <a href="#">
                    Get Free Quote &rarr;
                </a>
            </div>
            <div class="col ms_box">
                <div class="ms_img">
                    <img src="../../assets/img/home-2-image-box-03.png" alt="">
                </div>
                <div class="ms_title2">
                    Multimedia Channels
                </div>
                <div class="ms_subtitle1">
                    We provide study materials with various formats: video, audio, slides, doc, prints, books and applications.
                </div>
                <a href="#">
                    Start now &rarr;
                </a>
            </div>
        </div>
    </div>
</div>
</template>

<script>
export default {
    name: 'Benefits'
}
</script>

<style scoped lang="scss">
@import '../../assets/style/variables.scss';


    .ms_benefits{
        margin: 100px 0;


        .ms_subtitle{
            text-transform: uppercase;
        }
        .ms_color{
            color: $color3;
            font-weight: normal;
            font-family: 'Roboto', serif;
        }

        .ms_box{
            margin-top: 50px;

            .ms_title2{
                font-size: 20px;
                margin-top: 30px;
                font-weight: bold;
            }
            .ms_subtitle1{
                margin: 20px 0;
                font-size: 17px;
            }
            a{
                color: $color13;
                text-decoration: none;
                font-weight: bold
            }
        }
    }
</style>