<template>
<section>
<h1>{{ message }}</h1>
<p>id: {{ this.$route.params.id }}</p>
</section>
</template>

<script>
export default{
    data: function(){
        return{
            message:'ss/_id.vue',
        };
    }
}
</script>
