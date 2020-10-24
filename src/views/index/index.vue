<template>
  <div class="amap-wrap">
    <el-amap
        vid="amapDemo"
        class="amap-demo"
        :zoom="zoom"
        :center="center"
    >
    </el-amap>
  </div>
</template>
<script>
export default {
  name: "index",
  data(){
    return{
      zoom:15,
      center:[116.397451,39.909187]
    }
  }
}
</script>
<style lang="scss">
.amap-wrap{
  height: 100vh;
}
</style>