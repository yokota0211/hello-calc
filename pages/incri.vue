<template>
 <div class="container">
   <button @click="increase">increase</button>
   <button @click="decrease">decrease</button>
   {{ $store.state.counter }}
 </div>
</template>

<script>
export default {
 methods: {
   increase () {
     this.$store.commit('increase')
   },
   decrease () {
    this.$store.commit('decrease')
   },
 },
}
</script>