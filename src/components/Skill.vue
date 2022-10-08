<template>
  <div class="flex column skill-single2">
    <p class="text-primary text-bold">{{title}}</p>
    <div class="flex nowrap">
        <div v-for="item in level" :key="item" class="icon-level text-accent">
            <i class="fa fa-star"></i>
        </div>
    </div>
  </div>
</template>

<script>
export default {
    name: 'SkillSingle',
    props: {
        title: String,
        level: Number
    }
}
</script>

<style>
    .skill-single2{
        width: 100%;
        margin-bottom: 25px;
    }
    .skill-single2 p{
        margin-bottom: 5px;
        font-size: 13px;
    }
    .skill-single2 .icon-level{
        font-size: 12px;
        margin-right: 3px;
    }

    @media screen and (max-width: 500px){
       .skill-single2 {
            align-items: center;
            padding-top: 15px;
       }
    }

</style>