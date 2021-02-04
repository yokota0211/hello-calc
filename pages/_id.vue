<template>
<section>
 <h1>{{message}}</h1>
<p>受け取ったid: {{ this.$route.params.id}}</p>
</section>
</template>

<script>
export default{
    data: function(){
        return{
            message:'_id.vueでパラメータを受け取りました',
        }
    }
}
</script>


<style>
p {
 font-size: 20px;
 background-color: silver;
}
</style>