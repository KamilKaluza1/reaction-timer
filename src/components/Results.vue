<template>
   <p> Score {{ score }} - ms</p> 
   <p>{{ comment }}</p>
</template>

<script>
export default {
    props:['score'],
    data() {
        return{
            comment: null
        }
    },
    mounted() {
        if(this.score < 250){this.comment="You are speed"}else if
        (this.score < 350){this.comment="You are ok"}else
        {this.comment= "Slow.."}
    }
}


</script>

<style>

</style>