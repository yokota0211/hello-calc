<template>
<section>
<p>足される数: {{ this.$route.params.add1}}</p>
<p>足す数: {{ this.$route.params.add2}}</p>
<p>計算式: {{ this.$route.params.add1+"+"+this.$route.params.add2+"="}}</p>
<button @click="answer">答えは</button>
<p>{{ message }}</p>
</section>
</template>

<script>
export default{
    data: function(){
        return{
            message:'calc/_add1/_add2/_ans.vue',
        };
    },
    methods: {
        answer(){
            this.message = this.$route.params.add1 + this.$route.params.add2
        },
    },
}
</script>