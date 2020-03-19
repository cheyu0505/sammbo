<template>
  <div class="morelistitem">
    <div class="morelist-item" ref="item" @click="click">
      {{item}}
      <img v-show="typeof this.detail=='object'" ref="arrow" src="../assets/img/下拉箭头.svg" alt />
    </div>
    <div class="morelist-detail" v-if="isshow">
      <div class="morelist-detail-item" v-for="(v,i) in detail" :key="i">
        {{v.item}}
        <span style="float:right">{{v.text}}</span>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  props: ["item", "detail"],
  data() {
    return {
      isshow: false
    };
  },
  mounted(){
    // console.log(typeof this.detail=="object")
  },
  methods: {
    click() {
      this.isshow = !this.isshow;
      if (this.isshow === true&&this.detail) {
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
.morelist-detail-item {
  width: 100%;
  height: 56px;
  padding: 0 40px;
  box-sizing: border-box;
  line-height: 56px;
  font-family: "PingFangSC-Regular";
  font-size: 14px;
  color: #6c6f6e;
  text-align: left;
}
</style>