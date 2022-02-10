<template>
<div class="ms_blog">
    <div class="ms_container">
        <div class="row row-cols-3">
            <div class="ms_text col">
                <div class="ms_subtitle">
                    Enjoyable insights
                </div>
                <div class="ms_title1">
                    Most Viewed
                    <span class="ms_color1">
                        Best Blogs
                    </span>
                </div>
                <div class="ms_title2">
                    <ul v-for="(element, index) in blog" :key="index">
                        <span>
                            &rarr;   
                        </span>
                        <li>
                            {{element.title}}
                        </li>
                    </ul>
                </div>
            </div>
            <div class="col ms_col" v-for="(element, index) in blogPreview" :key="index">
                <div class="ms_box">
                    <div class="ms_img">
                        <img :src="element.img" alt="">
                    </div>
                    <div class="ms_text">
                        <div class="ms_subtitle">
                            {{element.artist}}
                        </div>
                        <div class="ms_title2">
                            {{element.title}}
                        </div>
                        <div class="ms_subtitle1">
                            <span class="ms_date">
                                <span class="ms_icon">
                                    <i class="ms_icon fas fa-calendar"></i>
                                </span>
                                {{element.date}}
                            </span>
                            <span>
                                <span class="ms_icon">
                                    <i class="fas fa-eye"></i>
                                </span>
                                {{element.views}}
                            </span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>
</template>

<script>
export default {
    name: 'Blog',
    data(){
        return{
            blog:[
                {
                    title:"Become a Better Blogger:Content Planning"
                },
                {
                    title:"Promoting Your Online Business on Pintarest"
                },
                {
                    title:"Gamification and Game-Based Learning"
                },
                {
                    title:"Designing an Online Course from Expert's Perspective"
                },
                {
                    title:"Why Online Courses Are the Future of Education"
                }
            ],
            blogPreview:[
                {
                    img: require("../../assets/img/artist-blog-03-480x352.jpeg"),
                    artist: "Artist",
                    title: "Brush Strokes Energize Trees in Paintings",
                    date: "May 15, 2020",
                    views: "688 views"
                },
                {
                    img: require("../../assets/img/artist-blog-01-480x352.jpg"),
                    artist: "Artist",
                    title: "Pocket-Sized Notebooks Hold Miniature Paintings",
                    date: "May 15, 2020",
                    views: "603 views"
                }
            ]
        }
    }
}
</script>

<style scoped lang="scss">
@import '../../assets/style/variables.scss';

    .ms_blog{
        background-color: $mycolor2;

        .ms_container{
            padding: 100px 0 50px;

            .ms_subtitle{
                text-transform: uppercase;
                margin-top: 40px;
            }
            .ms_title1{
                font-size: 33px;

                .ms_color1{
                    font-weight: normal;
                }
            }
            .ms_title2{
                font-size: 15px;
                margin-top: 30px;
                ul{
                    padding-left: 0;
                    margin-top: 25px;

                    span{
                        vertical-align: top;
                        margin-right: 10px;
                    }

                    li{
                        list-style: none;
                        display: inline-block;
                        width: 300px;
                    }
                }
            }
            .ms_col{
                padding: 30px;

                .ms_box{
                    background-color: $color0;
                    border-radius: 5px;
                    
                    
                    
    
                    .ms_img{
                        height: 250px;
    
                        img{
                            width: 100%;
                            height: 100%;
                            border-radius: 5px 5px 0 0;
                            object-fit: cover;
                        }
                    }
                    .ms_text{
                        padding: 30px 40px;
                    }
                    .ms_subtitle{
                        margin: 0;
                    }
                    .ms_title2{
                        margin: 10px 0 20px;
                        font-size: 20px;
                    }
                    .ms_subtitle1{
                        font-size: 15px;
                        .ms_date{
                            margin-right: 40px;
                        }
                        .ms_icon{
                            margin-right: 5px;
                        }
                    }
                }
            }
        }
    }

</style>