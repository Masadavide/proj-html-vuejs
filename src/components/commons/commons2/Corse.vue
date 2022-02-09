<template>
    <div>
        <div class="col-6 d-flex align-items-center ms_box" v-for="(element, index) in links" :key="index">
            <div class="ms_img">
                <img :src="element.img" alt="">
            </div>
            <div class="ms_text">
                <div class="ms_price">
                    {{element.cost}}
                </div>
                <div class="ms_title2">
                    {{element.text}}
                </div>
                <div class="ms_info ms_subtitle">
                    <span class="students">
                        <i class="far fa-file-alt ms_icon"></i>
                        {{element.lession}}
                    </span>
                    <span>
                        <i class="far fa-user ms_icon"></i>
                        {{element.students}}
                    </span>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Corse',
    data(){
        return{
            links:[
                {
                    img: require("../../../assets/img/course-02-480x298.jpg"),
                    cost: "$40.00",
                    text: "Learning to Write as a Professional Author",
                    lession: "20 Lessons",
                    students: "50 Students"
                },
                {
                    img: require("../../../assets/img/stock-full-hd-03-480x298.jpg"),
                    cost: "Free",
                    text: "Customer-centric Info-Tech Strategies",
                    lession: "24 Lessons",
                    students: "769 Students"
                },
                {
                    img: require("../../../assets/img/stock-full-hd-04-480x298.jpg"),
                    cost: "$19.00",
                    text: "Open Programming Courses for Everyone: Python",
                    lession: "17 Lessons",
                    students: "62 Students"
                },
                {
                    img: require("../../../assets/img/stock-full-hd-06-480x298.jpg"),
                    cost: "$26.00",
                    text: "Academic Listening and Note-taking",
                    lession: "14 Lessons",
                    students: "67 Students"
                },
                {
                    img: require("../../../assets/img/course-featured-image-01-480x298.jpg"),
                    cost: "$39.00",
                    text: "Master jQuery in a Short Period of Time",
                    lession: "6 Lessons",
                    students: "51 Students"
                },
                {
                    img: require("../../../assets/img/stock-full-hd-05-480x298.jpg"),
                    cost: "$59.00",
                    text: "Introduction to Javascript for Beginners",
                    lession: "14 Lessons",
                    students: "76 Students"
                }
            ]
        }
        
    }
}
</script>

<style lang='scss' scoped>
@import '../../../assets/style/variables.scss';

.ms_box{
    margin-top: 60px;

    .ms_img{
        width: 150px;
        height: 150px;

        img{
            width: 100%;
            height: 100%;
            border-radius: 100%;
            object-fit: cover;
        }
    }

    .ms_text{
        padding-left: 30px;
        width: 350px;

        .ms_price{
            color: $color3;
            font-size: 25px;
            font-weight: bold;
        }
        .ms_info{
            font-size: 13px;
            margin-top: 10px;

            .students{
                margin-right: 25px;
            }
            
        }
    }
}
    
    
    .ms_icon{
        margin-right: 10px;
    }

</style>