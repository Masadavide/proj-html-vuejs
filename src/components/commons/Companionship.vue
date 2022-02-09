<template>
<div class="ms_companionship">
    <div class="ms_container">
        <div class="row row-cols-2">
            <div class="col">
                <div class="img">
                    <img class="image" src="../../assets/img/home-2-popup-video-poster.jpg" alt="">
                    <img class="ms_yt" src="../../assets/img/icon-youtube-play.png" alt="">
                </div>
            </div>
            <div class="col ms_box">
                <div class="ms_subtitle">
                    Get started 
                    <span class="ms_color">
                        Effortlessly
                    </span>
                </div>
                <div class="ms_title">
                    Enjoy Our 
                    <span class="ms_color1">
                        Companionship
                    </span>
                </div>
                <div class="ms_subtitle1">
                    Sneek peek into what has in store for you on our online teaching and mentoring portal. Seek for some hidden hints of early-bird rewards as well.
                </div>
                <a href="#">
                    Download free guidebook &rarr;
                </a>
            </div>
        </div>
    </div>
</div>
</template>

<script>
export default {
    name: 'Companionship',
}
</script>

<style scoped lang="scss">
@import '../../assets/style/variables.scss';

    .ms_companionship{
        padding: 100px 0;
        border-top: none;
        box-shadow: 800px 10px 0px 0px $mycolor;
        border-radius: 0 0 50% 0;
        border-collapse: collapse;
        width: calc(100vw + 30px);
        
        .col{
            .img{
                position: relative;

                .image{
                    width: 100%;
                    height: 100%;
                }
                .ms_yt{
                    position: absolute;
                    top: 50%;
                    left: 50%;
                    transform: translate(-50%, -50%);
                }
            }
        }
        .ms_box{
            padding: 30px 125px 0;
            .ms_subtitle{
                text-transform: uppercase;
                font-weight: bold;
                margin-bottom: 20px;

            }
            .ms_title{
                .ms_color1{
                    font-weight: normal;
                }
            }
            .ms_subtitle1{
                margin-top: 30px;
                margin-bottom: 50px;
            }
            a{
                text-decoration: none;
                border-bottom: 1px solid $color2;
                padding-bottom: 2px;
                color: $color3;
                font-weight: bold;
            }
        }
    }

</style>