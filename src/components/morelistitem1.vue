<template>
  <div class="morelistitem">
    <div class="morelist-item" ref="item" @click="click">
      关注闪布
      <img ref="arrow" src="../assets/img/下拉箭头.svg" alt />
    </div>
    <div class="morelist-detail" v-if="isshow">
      <div class="morelist-detail-item1">
        <div class="detail-item-app">
          <div class="apptext">闪布APP</div>
          <img src="../assets/img/app.png" alt />
        </div>
        <div class="detail-item-app">
          <div class="apptext">闪布APP</div>
          <img src="../assets/img/app.png" alt />
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      isshow: false
    };
  },
  methods: {
    click() {
      this.isshow = !this.isshow;
      if (this.isshow === true) {
        this.$refs.item.style.background = "#F6F6F6";
        this.$refs.arrow.style.transform = "rotate(180deg)";
      } else {
        this.$refs.item.style.background = "#FFF";
        this.$refs.arrow.style.transform = "rotate(360deg)";
      }
    }
  }
};
</script>
<style>
.morelist-item {
  width: 100%;
  height: 72px;
  padding: 0 24px;
  box-sizing: border-box;
  font-family: "PingFangSC-Regular";
  font-size: 16px;
  color: #1d2221;
  line-height: 72px;
  display: flex;
  justify-content: space-between;
}
.morelist-detail {
  width: 100%;
}
.morelist-detail-item1 {
  width: 100%;
  height: 168px;
  padding: 0 40px;
  box-sizing: border-box;
  font-family: "PingFangSC-Regular";
  font-size: 14px;
  color: #6c6f6e;
  display: flex;
  justify-content: space-around;
}
.detail-item-app {
  width: 72px;
  text-align: center;
}
.apptext {
  margin-top: 28px;
  margin-bottom: 13px;
}
.morelist-detail-item1 img {
  width: 72px;
  height: 72px;
}
</style>