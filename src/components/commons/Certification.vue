<template>
<div>
    <div class="ms_certification">
        <div class="ms_container">
            <div class="ms_text text-center">
                <div class="ms_title2">
                    Start today for getting 
                    <span class="ms_color1">
                        Online Certification
                    </span>
                </div>
                <div class="ms_title">
                    You can be your own guiding star with our help!
                </div>
                <button>
                    Get started now
                </button>
            </div>
        </div>
    </div>
    <div class="ms_certification1">
        <div class="container">
            <div class="row row-cols-4">
                <div class="col ms_box text-center">
                    <div class="ms_title2">
                        Successfully trained
                    </div>
                    <div class="ms_number">
                        1790
                    </div>
                    <div class="ms_subtitle">
                        Enrolled learners
                    </div>
                </div>
                <div class="col ms_box text-center">
                    <div class="ms_title2">
                        Proudly Received
                    </div>
                    <div class="ms_number">
                        19
                    </div>
                    <div class="ms_subtitle">
                        Counterywide awards
                    </div>
                </div>
                <div class="col ms_box text-center">
                    <div class="ms_title2">
                        Firmly Established
                    </div>
                    <div class="ms_number">
                        24
                    </div>
                    <div class="ms_subtitle">
                        Local Braches
                    </div>
                </div>
                <div class="col ms_box ms_box1 text-center">
                    <div class="ms_title2">
                        Getting Featured on
                    </div>
                    <div class="ms_number">
                        1090
                    </div>
                    <div class="ms_subtitle">
                        Blog posts
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>
</template>

<script>
export default {
    name: 'Reviews'
}
</script>

<style scoped lang="scss">
@import '../../assets/style/variables.scss';

    .ms_certification{
        background-color: $mycolor;
        padding: 50px 0;

        button{
            margin: 50px 0;
            padding: 15px 80px;
        }
    }

    .ms_certification1{
        .row{

            .ms_box{
                padding: 100px 0;
                border-left: 4px solid $mycolor;
                .ms_title2{
                    margin-bottom: 20px;
                    padding: 0 100px;
                }
                .ms_number{
                    font-size: 50px;
                    font-weight: bold;
                    color: $color3;
                    font-family: 'Roboto Slab', serif;
                }
                .ms_subtitle{
                    text-transform: uppercase;
                }
            }
            .ms_box1{
                border-right: 4px solid $mycolor;
            }
        }
    }
    
</style>