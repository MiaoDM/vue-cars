<template>
  <div>
    <section class="cars-item">
      <header>
        <h4 class="cars-logo">
          <img src="../../assets/cars-logo.png" alt="Mustang 2019款"/>
          <span class="name">Mustang 2019款</span>
        </h4>
        <p class="cars-attr">新能源汽车 5座</p>
      </header>
      <div class="cars-content">
        <div class="info">
          <div>
            <h4 class="cars-number">粤 B745N8</h4>
            <div>
              <ul class="cars-power active-li-4">
                <li></li>
                <li></li>
                <li></li>
                <li></li>
                <li></li>
                <li></li>
                <li></li>
                <li></li>
                <li></li>
                <li></li>
              </ul>
              <p class="distance">
                <sub>约</sub>
                <strong>600</strong>
                <sub>KM</sub>
              </p>
            </div>
          </div>
        </div>
        <img src="../../assets/images/pic001.jpg" alt=""/>
      </div>
      <footer>
        <a href="javascript:void(0);" class="parking-link">某某停车场</a>
      </footer>
    </section>
    <section class="cars-item cars-detail" :style="'height:' + height">
      <div class="scroll">
        <h4 class="colume">某某停车场
          <i class="close"></i>
        </h4>
        <header>
          <h4 class="cars-logo">
            <img src="../../assets/cars-logo.png" alt="Mustang 2019款"/>
            <span class="name">Mustang 2019款</span>
          </h4>
          <p class="cars-attr">新能源汽车 5座</p>
        </header>
        <img src="../../assets/images/pic001.jpg" alt="" width="100%"/>
        <div class="clearfix clearfix">
          <h4 class="pull-left fs-24">粤 B745N8</h4>
          <p class="distance pull-right">
            <sub>约</sub>
            <strong>600</strong>
            <sub>KM</sub>
          </p>
        </div>
        <div class="cars-power-box">
          <div class="p-r">
            <span class="e-hight" style="width: 80%"></span>
            <span class="e-bg"></span>
          </div>
        </div>
        <p class="info color-main tetx-center">取车约支付12.0元停车费，实际补贴12.0元</p>
        <ul class="cars-type-checked">
          <li class="current">
            <h4 class="name">日租车</h4>
            <span class="price">￥ 300/1天</span>
          </li>
          <li>
            <h4 class="name">日租车</h4>
            <span class="price">￥ 300/1天</span>
          </li>
          <li>
            <h4 class="name">日租车</h4>
            <span class="price">￥ 300/1天</span>
          </li>
          <li>
            <h4 class="name">日租车</h4>
            <span class="price">￥ 300/1天</span>
          </li>
        </ul>
        <div class="clause-des">
          <span class="pull-left">参保《全面保障服务》用车更放心</span>
          <i class="current"></i>
        </div>
      </div>
      <a href="javascript:void(0);" class="select-car-btn">预约用车</a>
    </section>
  </div>
</template>
<script>
export default {
  name: "CarsList",
  props: {
    height: {
      type: String,
      default: "257px"
    }
  }
}
</script>
<style lang="scss">
@import "./index.scss";
</style>