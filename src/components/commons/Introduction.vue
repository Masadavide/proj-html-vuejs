<template>
<div class="ms_introduction">
    <div class="ms_container">
        <div class="d-flex align-items-center justify-content-between">
            <div class="ms_text">
                <div class="ms_title">
                    Distant learning for further expansion
                </div>
                <div class="ms_subtitle ms_subtitle-margin">
                    Learning is a life-long journey that in fact we never find the terminate stop. Stop searching, enjoy the process.
                </div>
                <button>
                    <i class="fas fa-download"></i>
                    Download free guide
                </button>
                <div class="ms_subtitle ms_subtitle-font">
                    Have question?
                    <a href="#">
                        Get Free Sample &rarr;
                    </a>
                </div>
            </div>
            <div class="ms_image">
                <img src="../../assets/img/about-me-profile-ohm4dxoearqbxny7q3bq1pzbdgofdx0tobbeqcvzd0.jpg" alt="">
            </div>
        </div>
        <div class="sponsor d-flex align-items-center justify-content-between">
            <img src="../../assets/img/client-logo-01.png" alt="">
            <img src="../../assets/img/client-logo-02.png" alt="">
            <img src="../../assets/img/client-logo-03.png" alt="">
            <img src="../../assets/img/client-logo-04.png" alt="">
            <img src="../../assets/img/client-logo-05.png" alt="">
            <img src="../../assets/img/client-logo-06.png" alt="">
        </div>
    </div>
</div>
</template>

<script>
export default {
    name: 'Introduction'
}
</script>

<style scoped lang="scss">
@import '../../assets/style/variables.scss';

.ms_introduction{
    margin: 50px 0;

    .d-flex{

        .ms_text{
            width: 400px;

            .ms_subtitle-margin{
                margin: 20px 0;
            }

            button{

                .fa-download{
                    margin-right: 5px;
                }
            }
            .ms_subtitle-font{
                font-size: 14px;
                margin: 20px 0;

                a{
                    color: $color3;
                    text-decoration: none;
                    margin-bottom: 2px;
                    border-bottom: 1px solid $color13;
                    padding-bottom: 2px;
                }
            }
            
        }
        .ms_image{
            width: 500px;
            
            img{
                width: 100%;
                height: 100%;
                border-radius: 100%;
            }
        }
    }
    .sponsor{
        margin-top: 50px;
    }
}

</style>