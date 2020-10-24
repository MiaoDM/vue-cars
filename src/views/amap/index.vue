<template>
  <div class="amap-wrap">
    <el-amap
        vid="amapDemo"
        class="amap-demo"
        :events="events"
    >
    </el-amap>
  </div>
</template>
<script>
import {lazyAMapApiLoaderInstance} from 'vue-amap';

export default {
  name: "Amap",
  data() {
    return {
      map:null,
      zoom: 15,
      events: {

      }
    }
  },
  mounted() {
    lazyAMapApiLoaderInstance.load().then(() => {
      // your code ...
      this.map = new AMap.Map('amapDemo', {
        center: new AMap.LngLat(116.397451, 39.909187),
        zoom:this.zoom, //初始化地图层级
      });
    });
  },
}
</script>
<style lang="scss">
.amap-wrap {
  height: 100vh;
}
</style>