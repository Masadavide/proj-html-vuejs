<template>
<div class="ms_reviews">
    <div class="ms_container">
        <div class="ms_subtitle text-center">
            Great words about maxcoach
        </div>
        <div class="ms_title text-center">
            Our 
            <span class="ms_color1">
                top learners'
            </span>
            verbatim
        </div>
    </div>
    <div class="row row-cols-3 ms_row">
        <div class="col ms_opacity" v-if="this.i == 0">
            <div class="ms_box">
                <div class="ms_title2">
                    It'a a choice of quality for people with special needs
                </div>
                <div class="ms_subtitle">
                    I'm a very stict person so I require everything to be organized and neat. Then, I'll be able to make things right and shine. MaxChoach guys just got me.
                </div>
                <div class="ms_user d-flex align-items-center">
                    <div class="ms_img">
                        <img src="../../assets/img/testimonial-avata-03.jpg" alt="">
                    </div>
                    <div class="ms_text">
                        <div class="ms_title2">
                            Florence Themes
                        </div>
                        <div class="ms_subtitle1">
                            / Multimedia Admin
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="col" :class="current(index)" v-for="(element, index) in review" :key="index">
            <div class="ms_box">
                <div class="ms_title2">
                    {{element.title}}
                </div>
                <div class="ms_subtitle">
                    {{element.text}}
                </div>
                <div class="ms_user d-flex align-items-center">
                    <div class="ms_img">
                        <img :src="element.img" alt="">
                    </div>
                    <div class="ms_text">
                        <div class="ms_title2">
                            {{element.name}}
                        </div>
                        <div class="ms_subtitle1">
                            {{element.profession}}
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="col ms_opacity" v-if="this.i == 3">
            <div class="ms_box">
                <div class="ms_title2">
                    High level of efficiency and scientific teaching method
                </div>
                <div class="ms_subtitle">
                    I am free to learn at my own pace, follow my own schedule and choose the subject i want to learn from the syllabus. Great study portal for people like me.
                </div>
                <div class="ms_user d-flex align-items-center">
                    <div class="ms_img">
                        <img src="../../assets/img/testimonial-avata-02.jpg" alt="">
                    </div>
                    <div class="ms_text">
                        <div class="ms_title2">
                            Mina Hollace
                        </div>
                        <div class="ms_subtitle1">
                            / Freelencer
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <div class="text-center">
        <span class="dots">
            <span class="dot" @click="i = index" :class="{active: index == i}" v-for="(element,index) in review" :key="index">
            </span>
        </span>
    </div>
</div>
</template>

<script>
export default {
    name: 'Reviews',
    data(){
        return{
            i: 0,
            review:[
                {
                    title: "High level of efficiency and scientific teaching method",
                    text: "I am free to learn at my own pace, follow my own schedule and choose the subject i want to learn from the syllabus. Great study portal for people like me.",
                    img: require("../../assets/img/testimonial-avata-02.jpg"),
                    name: "Mina Hollace",
                    profession: "/ Freelencer"
                },
                {
                    title: "Professional team of specialists and passionate mentors at reach",
                    text: "I need to get a certification for English proficiency and MaxCoach is my best choice. Their tutors are smart and professional when dealing with students.",
                    img: require("../../assets/img/testimonial-avata-04.jpg"),
                    name: "Madley Pondor",
                    profession: "/ IT Specialist"
                },
                {
                    title: "The perfect way to become Web Developer.",
                    text: "Boolean is the way to go to become Web Developer. Period. Their method is well estabilished, their teachers are well formed and passionate!",
                    img: require("../../assets/img/testimonial-avata-01.jpg"),
                    name: "Anonymous",
                    profession: "/ Full Stack Web Developer "
                },
                {
                    title: "It'a a choice of quality for people with special needs",
                    text: "I'm a very stict person so I require everything to be organized and neat. Then, I'll be able to make things right and shine. MaxChoach guys just got me.",
                    img: require("../../assets/img/testimonial-avata-03.jpg"),
                    name: "Florence Themes",
                    profession: "/ Multimedia Admin"
                }
            ]
        }
    },
    methods:{
        current: function(index){
            if(index == this.i || index == this.i + 1 || index == this.i - 1){ 
                if(index == this.i +1 || index == this.i - 1){
                    return "ms_opacity"
                }
                return "show"
            }
            return "noshow"
        },

    }
}
</script>

<style scoped lang="scss">
@import '../../assets/style/variables.scss';

    .ms_reviews{
        background-color: $mycolor;

        .ms_container{
            padding-top: 100px;

            .ms_subtitle{
                font-size: 22px;
                text-transform: uppercase;
            }

            .ms_color1{
                font-weight: normal;
            }
        }

        .ms_row{
            margin: 30px;
            
            ms-box1{
                margin-right: 12px;
            }

            .ms_box{
                background-color: $color0;
                padding: 50px;
                height: 410px;
                border-radius: 5px;
                

                .ms_subtitle{
                    margin: 20px 0;
                }
                .ms_user{
                    margin-top: 40px;

                    .ms_img{
                        width: 80px;
                        height: 80px;
                        display: inline-block;
                        img{
                            width: 100%;
                            height: 100%;
                            border-radius: 100%;
                        }
                    }
                }
                .ms_text{
                    display: inline-block;
                    margin-left: 20px;
                }
            }
        }
    }

    .dot{
        cursor: pointer;
        background-color: $color2;
        height: 8px;
        width: 8px;
        margin: 7px;
        border-radius: 50%;
        display: inline-block;
        transition: background-color 0.6s ease;
        vertical-align: middle;

        &:hover{
            background-color: $color12;
        }
        }

    .show{
        display: block;
    }
    .noshow{
        display: none;
    }

    .col{
        padding-left: 25px;
        padding-right: 25px;
    }

    .active{
        cursor: pointer;
        background-color: $color12;
        height: 12px;
        width: 12px;
        margin: 7px;
        border-radius: 50%;
        display: inline-block;
        transition: background-color 0.6s ease;
        vertical-align:auto;
    }

    .ms_opacity{
        opacity: 65%;
    }

</style>