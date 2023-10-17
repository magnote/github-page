<template>
  <div class="page">
    <Header></Header>
    <SiderBar class="side-bar"></SiderBar>
    <div class="pages">
      <router-view/>
    </div>
  </div>
</template>

<script setup>
  import Header from '@/components/header.vue'; 
  import SiderBar from '@/components/sider-bar.vue'; 

</script>



<style scoped>
.page {
  width: 100vw;
  height: 100vh;
  position: relative;
}

.side-bar {
  position: absolute;
  top: 70px;
  bottom: 0;
}


.pages {
  position: absolute;
  top: 80px;
  left: 190px;
  bottom: 0;
  right: 0;
}

</style>
