<template>
  <div>
          <div class="content">
      <div class="more">
        <div class="more-item">
          <div class="more-item-title">产品</div>
          <div class="more-item-detail">产品介绍</div>
        </div>
        <div class="more-item">
          <div class="more-item-title">行业场景</div>
          <div class="more-item-detail">
            <a href="/"><p>互联网/信息技术</p></a>
            <p>制造业/新零售</p>
            <p>供应链/外包产业</p> 
          </div>
        </div>
        <div class="more-item">
          <div class="more-item-title">服务</div>
          <div class="more-item-detail">
            <p>用户服务</p>
            <p>隐私权说明</p>
            <p>用户服务协议</p>
          </div>
        </div>
        <div class="more-item">
          <div class="more-item-title">支持</div>
          <div class="more-item-detail">
            <p>开发者平台</p>
            <p>关于我们</p>
          </div>
        </div>
        <div class="more-item">
          <div class="more-item-title">联系我们</div>
          <div class="more-item-detail">
            <p>咨询（工作日：9:00～18:00）</p>
            <p>联系电话</p>
            <span style="color: #1D2221;">13575719446</span>
            <p>支持邮箱</p>
            <span style="color: #1D2221;">thundbu@geely.com</span>
          </div>
        </div>
        <div class="more-item">
          <div class="more-item-title">关于闪布</div>
          <div class="more-item-detail">
            <p @mouseover="changeActive1">闪布APP</P>
            <img src="../assets/img/app.png" alt v-show="active==1" class="qr"/>
            <P @mouseover="changeActive2">闪布公众号</P>
            <img src="../assets/img/gongzhonghao.jpg" alt v-show="active==2" class="qr" />
          </div>
        </div>
      </div>
    </div>
    <div class="morelist">
      <morelistitem v-for="(v,i) in itemdata" :key="i" v-bind="v" />
      <morelistitem1 />
    </div>
    <div
      class="copyright"
    >Copyright © 2019 杭州闪布科技有限公司 浙ICP备16046364号-4 全国互联网安全管理平台 备案号：33010802010306</div>
  </div>
</template>
<script>
import morelistitem from "./morelistitem";
import morelistitem1 from "./morelistitem1";
export default {
  components:{
    morelistitem,
    morelistitem1
  },
  data(){
    return {
            itemdata: [
        { item: "产品", detail: [{ item: "产品介绍" }] },
        {
          item: "行业场景",
          detail: [
            { item: "互联网/信息与技术" },
            { item: "制造业/新零售" },
            { item: "供应链/外包服务业" }
          ]
        },
        {
          item: "联系我们",
          detail: [
            { item: "咨询电话（工作日：9:00～18:00）", text: "13575719446" },
            { item: "支持邮箱", text: "thunbu@geely.com" }
          ]
        }
      ],
      active: 2
    }
  },
  methods: {
    changeActive1() {
        this.active = 1;
    },
     changeActive2() {
        this.active = 2;
    }
  }
};
</script>
<style>
.more {
  width: 100%;
  height: 330px;
  display: flex;
  justify-content: space-between;
}
.more a {
  color: #6c6f6e;
}
.more-item {
  padding-top: 32px;
  box-sizing: border-box;
}
.more-item-title {
  margin-bottom: 26px;
  font-family: "PingFangSC-Regular";
  font-size: 16px;
  color: #1d2221;
  line-height: 24px;
  font-weight: 600;
}
.more-item-detail {
  font-family: "PingFangSC-Regular";
  font-size: 14px;
  color: #6c6f6e;
  line-height: 30px;
}
.more-item-detail p{
  color: #6c6f6e;
}
.copyright {
  font-family: "PingFangSC-Regular";
  font-size: 12px;
  color: #6c6f6e;
  line-height: 20px;
  text-align: center;
  margin-bottom: 12px;
  padding: 0 24px;
  box-sizing: border-box;
}
.morelist {
  display: none;
  width: 100%;
}
@media screen and (min-width: 1201px) {
  .content {
    width: 1136px;
    margin: 0 auto;
  }
}
@media screen and (min-width: 992px) and (max-width: 1200px) {
  .content {
    width: 942px;
    margin: 0 auto;
  }
}
@media screen and (min-width: 768px) and (max-width: 992px) {
  .content {
    width: 100%;
    margin: 0 auto;
    padding: 0 16px;
    box-sizing: border-box;
  }
}
@media screen and (max-width: 768px) {
  .content {
    width: 100%;
    padding: 0 24px;
    box-sizing: border-box;
    margin: 0 auto;
  }
  .more {
    display: none;
  }
  .copyright {
    margin-top: 48px;
  }
  .morelist {
    display: block;
  }
}
</style>