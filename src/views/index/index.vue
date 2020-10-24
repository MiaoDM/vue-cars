<template>
  <div>
    <!--    地图-->
    <Map/>
    <!--    导航-->
    <Navbar/>
    <!--    cars data渲染-->
    <Cars/>
    <!--  会员-->
    <!--    <div id="children-view" :class="[show?'open':'']">-->
    <div id="children-view" :class="{open:show}">
      <router-view/>
    </div>

  </div>
</template>
<script>
import Map from "../amap";
import Cars from "../cars";
import Navbar from "@c/navbar";

export default {
  name: "index",
  components: {Cars, Map,Navbar},
  data() {
    return {
      // show: false,
    }
  },
  computed: {
    show() {
      const router = this.$route;
      return router.name == "Index" ? false : true;
    }
  },
  watch: {
    // "$route": {
    //   handler(newValue) {
    //     const rouerName = newValue.name;
    //     this.show = rouerName == "Index" ? false : true;
    //     // console.log(this.show);
    //   }
    // }
  }
}
</script>
<style lang="scss">
#children-view {
  position: fixed;
  top: 0px;
  bottom: 0px;
  right: -600px;
  z-index: 101;
  width: 410px;
  background-color: #34393f;
  -webkit-transition: all .3s ease 0s;
  -moz-transition: all .3s ease 0s;
  -ms-transition: all .3s ease 0s;
  -o-transition: all .3s ease 0s;
  transition: all .3s ease 0s;

  &.open {
    right: 0px;
  }
;

}
</style>