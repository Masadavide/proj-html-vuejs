<template>
<div class="ms_footer">
    <div class="ms_container">
        <div class="row row-cols-2">
            <div class="col">
                <div class="ms_title2">
                    Address
                </div>
                <ul class="ms_subtitle1">
                    <li>
                        382 NE 191st St # 87394 Miami, Fl 33179-3899
                    </li>
                    <li>
                        +1 (305) 547-9909 (9am - 5pm EST, Monday - Friday)
                    </li>
                    <li>
                        support@maxcoach.com
                    </li>
                    <div>
                        <span class="ms_icon">
                            <i class="fab fa-facebook-square"></i>
                        </span>
                        <span class="ms_icon">
                            <i class="fab fa-twitter"></i>
                        </span>
                        <span class="ms_icon">
                            <i class="fab fa-instagram"></i>
                        </span>
                        <span class="ms_icon">
                            <i class="fab fa-linkedin"></i>
                        </span>
                    </div>
                </ul>
            </div>
            <div class="col">
                <div class="row row-cols-2">
                    <div class="col ">
                        <div class="ms_title2">
                            Explore
                        </div>
                        <div class="row row-col-2 ms_col">
                            <ul class="ms_subtitle1 col">
                                <li>
                                    Start here
                                </li>
                                <li>
                                    Blog
                                </li>
                                <li>
                                    About us
                                </li>
                            </ul>
                            <ul class="ms_subtitle1 col">
                                <li>
                                    Success story
                                </li>
                                <li>
                                    Courses
                                </li>
                                <li>
                                    Contact us
                                </li>
                            </ul>
                        </div>
                    </div>
                    <div class="col">
                        <div class="ms_title2">
                            Information
                        </div>
                        <ul class="ms_subtitle1">
                            <li>
                                Membership
                            </li>
                            <li>
                                Purchase guide
                            </li>
                            <li>
                                Privacy policy
                            </li>
                            <li>
                                Term of services
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
        <div class="ms_subtitle1 ms_rights text-center">
            © 2020 Maxcoach. All Rights Reserved
        </div>
    </div>
    <a class="ms_arrow" @click="scrollToTop()">&uarr;</a>
</div>
</template>

<script>
export default {
    name: 'Footer',
    methods: {
        scrollToTop() {
            window.scrollTo(0, 0);
        }
    }
}
</script>

<style scoped lang="scss">
@import '../../assets/style/variables.scss';

    .ms_footer{
        background-color: $mycolor;
        padding: 70px 0 40px;

        .ms_icon{
            margin-right: 20px;
            cursor: pointer;

            &:hover{
            color: $color3;
            }
        }
    }


    ul{
        padding: 0;
    }
    li{
        list-style: none;
        margin: 10px 0;
        color: $color13;
        cursor: pointer;
        &:hover{
            color: $color3;
        }
    }
    .ms_col{
        padding-left: 12px;
    }
    .ms_rights{
        margin-top: 50px;
    }
    .ms_arrow{
        float: right;
        text-decoration: none;
        background-color: $color3;
        border-radius: 100%;
        padding: 10px 23px;
        color: $color0;
        font-size: 25px;
        cursor: pointer;
        margin-top: -50px;
        margin-right: 30px;

        &:hover{
            background-color: $color19;
        }
    }


</style>