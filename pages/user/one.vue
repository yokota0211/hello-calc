<template>
<section>
 <h1>{{title}}</h1>
 <p>{{message}}</p>

 <NuxtLink to="/">Topへ</NuxtLink>
 <NuxtLink to="/user/">userのTopへ</NuxtLink>
 <NuxtLink to="/user/two">userのtwoへ</NuxtLink>

</section>
</template>

<script>
export default {
  data: function(){
    return{
      title:'/user/one.vue',
      message: 'こちらはuserディレクトリのone.vueです',
    };
  },
};

</script>

<!---->
<style>
h1{
    font-size:10pt;
    color:#0000ff;
}
p{
    font-size: 20pt;
}
</style>