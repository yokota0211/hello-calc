<template>
<section>
 <h1>{{title}}</h1>
 <p>{{message}}</p>

 <NuxtLink :to="{ name: 'index' }">Topへ</NuxtLink>
 <NuxtLink :to="{ name: 'user-one' }">userのoneへ</NuxtLink>
 <NuxtLink :to="{ name: 'user-two' }">userのtwoへ</NuxtLink>

</section>
</template>

<script>
export default {
  data: function(){
    return{ 
      title: '/user/index.vueです',
      message: 'こちらはuserディレクトリのTopページです',
    };
  },
};
</script>

<style>
.container {
  padding-top:5px;
  font-size: 5pt;
}
h1{
    font-size: 30pt;
    color: #ff0000;
}
p{
    font-size: 10pt;
}
</style>