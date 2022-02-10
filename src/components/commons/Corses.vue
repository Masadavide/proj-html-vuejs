<template>
<div class="ms_corses">
    <div class="ms_container">
        <div class="ms_subtitle text-center">
            Stimulated to learn?
        </div>
        <div class="ms_title1 text-center">
            Featured Online Courses
        </div>

        <Corse class="row ms_corse justify-content-between"/>

        <div class="ms_btn">
            <button>
                View all courses &rarr;
            </button>
        </div>
    </div>
</div>
</template>

<script>
import Corse from "./commons2/Corse.vue"

export default {
    name: 'Corses',
    components: {
        Corse
    }
}
</script>

<style scoped lang="scss">
@import '../../assets/style/variables.scss';
.ms_corses{
    background-color: $mycolor;
    padding: 100px 0;

    .ms_subtitle{
        text-transform: uppercase;
        margin-bottom: 10px;
    }
    .ms_corse{
        margin: 70px 0;
    }

    button{
        display: block;
        margin: 0 auto;
        padding: 15px 80px;
    }
}


</style>