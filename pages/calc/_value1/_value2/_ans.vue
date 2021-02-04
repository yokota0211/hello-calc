<template>
<section>
<p>数値１: {{ this.$route.params.value1}}</p>
<p>数値２: {{ this.$route.params.value2}}</p>
<p>掛け算: {{ this.$route.params.value1+"*"+this.$route.params.value2+"="}}</p>
<p><button @click="answer">答えは →</button>{{ message }}</p>
</section>
</template>

<script>
export default{
    validate({ params }) {
       if (params.value1 == undefined || params.value2 == undefined){
            return false // Nuxt.js にルートをレンダリングさせるのを止め、エラーページを表示させます
       } else {
            return true;
       }
    },
    data: function(){
        return{
            message:'calc/_value1/_value2/_ans.vue',
        };
    },
    methods: {
        answer(){
            this.message = this.$route.params.value1 * this.$route.params.value2
        },
    },

}
</script>