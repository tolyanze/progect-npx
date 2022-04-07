<template>
  <div class="wrapper">

    <vueHeader :links="links"/>

    <div class="wrapper-content">
      <div class="container">
        <h2>Content </h2>
      </div>
    </div>

    <vueFooter :links="links"/>

  </div>
</template>

<style lang="scss">
  
</style>

<script>
import vueHeader from '@/components/vue-Header'
import vueFooter from '@/components/vue-Footer'
export default {
  components:{vueHeader, vueFooter},
  data(){
    return{
      links:[
        {
          title: "Home",
          alias: "Home",
          url: "/"
        },
        {
          title: "About",
          alias: "About",
          url: "/about"
        }
      ]
    }
  }  
}
</script>
