<template>
<section>
<h1>{{ message }}</h1>
<p>tel: {{ this.$route.params.tel }}</p>
<p>name: {{ this.$route.params.name }}</p>
</section>
</template>

<script>
export default{
    data: function(){
        return{
            message:'_name.vueでtelとnameパラメータを受け取りました',
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