<template>
<div class="ms_newslatter">
    <div class="ms_container text-center row">
        <div class="col-6 m-auto">
            <div class="ms_title1">
                Subscribe 
                <span class="ms_color1">
                    Newsletter
                </span>
            </div>
            <div class="ms_subtitle">
                Enter your email address to register to our newslatter subscription delivered on a regular basis!
            </div>
            <div class="ms_input">
                <div class="input-group mb-3">
                    <input type="text" class="form-control" placeholder="Enter your email">
                    <button class="btn btn-outline-secondary" type="button">Subscribe</button>
                </div>
            </div>
        </div>
    </div>
</div>
</template>

<script>
export default {
    name: 'Newsletter',
    
}
</script>

<style scoped lang="scss">
@import '../../assets/style/variables.scss';

    .ms_newslatter{
        padding: 70px 0;

        .ms_color1{
            font-weight: normal;
        }

        .ms_subtitle{
            padding: 30px 0 40px;
            font-size: 18px;
        }

        .ms_input{

            input{
                background-color: $mycolor;
                color: $color2;
                padding-left: 20px;
                border: 0;
            }

            button{
                background-color: $color3;
                color: $color0;
                font-size: 13px;
                font-weight: bold;
                padding: 15px 40px;
                border: 0;
            }
        }
    }

</style>