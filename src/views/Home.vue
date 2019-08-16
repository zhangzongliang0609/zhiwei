<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
   <h1 ref="ddo" v-for="(elem,i) of qq" :key="i">你？？？？？？？</h1>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'home',
  components: {
    HelloWorld
  },
  data(){
    return {
     qq:[0,1,2,3,4,5,6,]
    }
  },
  methods:{

  },
  created:function(){
    console.log(this.$refs);
  },
  mounted:function(){
      console.log(this.$refs.ddo[0].innerHTML);
  }
}
</script>
