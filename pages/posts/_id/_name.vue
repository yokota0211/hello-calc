<template>
<section>
<h1>{{ message }}</h1>
<p>id: {{ this.$route.params.id}}</p>
<p>name: {{ this.$route.params.name}}</p>
</section>
</template>

<script>
export default{
    data: function(){
        return{
            message:'posts/_id/_name.vue',
        };
    }
}
</script>