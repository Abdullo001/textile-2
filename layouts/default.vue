<template>
 <div class="site-wrapper">
  <div class="sidebar">
    <Sidebar/>
  </div>
  <div class="main-wrapper">
    <Header />

    <div>
      <v-container>
        <nuxt/>
      </v-container>
    </div>
  </div>
 </div>
</template>

<script>
import Sidebar from '../components/Sidebar.vue';
import Header from '../components/Header.vue';
export default {
  name: "DefaultLayout",

  components:{
    Sidebar,Header,
  }

  

};
</script>

<style scoped lang="scss">
.site-wrapper{
  display: flex;
  background-color: #dfdfdf;
  min-height: 100vh;
}
.main-wrapper{
  flex-grow: 2;
}

</style>
