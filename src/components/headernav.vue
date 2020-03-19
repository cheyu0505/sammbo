<template>
  <div class="nav" ref="headernav">
    <div class="header-nav clearfix">
      <div class="header-nav-left">
        <a href="/" class="logo-container">
          <img src="../assets/img/logo1.png" alt />
          <img src="../assets/img/logo_text.png" alt />
        </a>
        <a href>
          <div class="header-nav-item">
            <span>产品</span>
          </div>
        </a>
        <div class="header-nav-item">
          <span style="margin-right:4px">行业场景</span>
          <i class="iconfont icon-zhaoshangxiaochengxu-jiantou-xia iconxia"></i>
          <div class="pullbox" v-if="pullboxflag">
            <a href>
              <div class="pullbox-item">互联网/信息与技术</div>
            </a>
            <div class="pullbox-item">制造业/新零售</div>
            <div class="pullbox-item">供应链/外包服务业</div>
          </div>
        </div>
        <a href>
          <div class="header-nav-item">
            <span>下载</span>
          </div>
        </a>
        <div class="header-nav-item">
          <span style="margin-right:4px">支持</span>
          <!-- <i class="iconfont icon-zhaoshangxiaochengxu-jiantou-xia"></i> -->
        </div>
      </div>
      <div class="header-nav-right">
        <div class="phonenum">
          <i class="iconfont icon-dianhua"></i>
          <span style="margin-left:7px">13575719446</span>
        </div>
        <div class="catalogbtn" @click="catalogisshow=!catalogisshow">
          <i class="iconfont icon-caidan" v-if="!catalogisshow"></i>
          <i class="iconfont icon-daochushujufuzhi" v-if="catalogisshow"></i>
        </div>
        <div class="catalog" v-if="catalogisshow">
          <morelistitem v-for="(v,i) in catalogdata" :key="i" v-bind="v" />
          <div class="catalog-freebtn">免费使用</div>
        </div>
        <span class="line" style="margin-left: 24px;color:#EBEBEB">|</span>
        <a href>
          <div class="header-nav-item">
            <span>登录</span>
          </div>
        </a>
        <div class="free-btn">免费使用</div>
      </div>
    </div>
  </div>
</template>
<script>
import morelistitem from "./morelistitem";
export default {
  name: "headernav",
  components: {
    morelistitem
  },
  data() {
    return {
      pullboxflag: false,
      catalogisshow: false,
      catalogdata: [
        { item: "首页" },
        { item: "产品", detail: [{ item: "产品介绍" }] },
        {
          item: "行业场景",
          detail: [
            { item: "互联网/信息与技术" },
            { item: "制造业/新零售" },
            { item: "供应链/外包服务业" }
          ]
        }
      ]
    };
  },
  mounted() {
    var headernav = this.$refs.headernav;
    window.onscroll = function() {
      headernav.style.boxShadow = "0 4px 8px 0 rgba(0,0,0,.06)";
      if (document.documentElement.scrollTop == 0) {
        headernav.style.boxShadow = "none";
      }
    };
    var navitem = document.querySelectorAll(".header-nav-item");
    var iconxia = document.querySelector(".iconxia");
    var _this = this;
    navitem.forEach(function(v, i) {
      v.onclick = function() {
        if (_this.pullboxflag === true) {
          navitem[1].classList.remove("active");
          iconxia.style.transform = "rotate(360deg)";
        } else {
          iconxia.style.transform = "rotate(180deg)";
          v.classList.add("active");
        }
        if (i == 1) {
          _this.pullboxflag = !_this.pullboxflag;
        }
      };
    });
  }
};
</script>
<style>
.catalogbtn {
  width: 24px;
  height: 24px;
  margin-left: 24px;
  float: right;
  display: none;
}
.catalogbtn .iconfont {
  font-size: 24px;
}
.catalog {
  width: 100%;
  height: 678px;
  position: fixed;
  top: 71px;
  left: 0;
  background-color: #fff;
}
.catalog-freebtn {
  margin: 0 auto;
  width: 356px;
  height: 40px;
  background: #7bf8d8;
  border-radius: 20px;
  text-align: center;
  line-height: 40px;
  margin-top: 40px;
}
.active {
  color: #25d3a7;
  border-bottom: 2px solid #25d3a7;
  box-sizing: border-box;
}
.nav {
  width: 100%;
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  margin: auto;
  background-color: #fff;
}
.header-nav-right a {
  display: block;
  height: 100%;
  line-height: 72px;
}
.header-nav-item {
  float: left;
  padding: 0 24px;
  box-sizing: border-box;
  display: flex;
  align-items: center;
  position: relative;
}
.header-nav-item img {
  margin-left: 4px;
  width: 14px;
}
.pullbox {
  width: 200px;
  position: absolute;
  top: 74px;
  left: 0;
  padding: 10px 0;
  box-sizing: border-box;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.15);
  background-color: #fff;
}
.pullbox-item {
  width: 100%;
  height: 48px;
  padding-left: 24px;
  box-sizing: border-box;
  font-family: "PingFangSC-Regular";
  font-size: 14px;
  color: #6c6f6e;
  line-height: 48px;
}
.pullbox-item:hover {
  background-color: #f6f6f6;
}
@media screen and (min-width: 1200px) {
  .header-nav {
    width: 1136px;
    height: 72px;
    color: #1d2221;
    font-size: 16px;
    margin: 0 auto;
  }
  .header-nav a {
    color: #1d2221;
  }
  .header-nav-left {
    height: 100%;
    float: left;
    line-height: 72px;
  }
  .logo-container {
    display: block;
    width: 157px;
    height: 100%;
    display: flex;
    align-items: center;
    float: left;
  }
  .logo-container img {
    height: 44px;
  }

  .header-nav-right {
    height: 100%;
    float: right;
    display: flex;
    align-items: center;
  }
  .free-btn {
    width: 96px;
    height: 36px;
    background-color: #7bf8d8;
    border-radius: 20px;
    float: right;
    font-size: 16px;
    line-height: 36px;
    text-align: center;
  }
  .phonenum {
    float: right;
    font-size: 22px;
    line-height: 72px;
    font-family: "PingFangSC-Medium";
    font-weight: 600;
  }
  .catalog {
    display: none;
  }
}

@media screen and (min-width: 992px) and (max-width: 1200px) {
  .header-nav {
    width: 942px;
    height: 72px;
    color: #1d2221;
    font-size: 16px;
    margin: 0 auto;
  }
  .header-nav a {
    color: #1d2221;
  }
  .header-nav-left {
    height: 100%;
    float: left;
    line-height: 72px;
  }
  .logo-container {
    display: block;
    width: 157px;
    height: 100%;
    display: flex;
    align-items: center;
    float: left;
  }
  .logo-container img {
    height: 44px;
  }
  .header-nav-right {
    height: 100%;
    float: right;
    display: flex;
    align-items: center;
  }
  .free-btn {
    width: 96px;
    height: 36px;
    background-color: #7bf8d8;
    border-radius: 20px;
    float: right;
    font-size: 16px;
    line-height: 36px;
    text-align: center;
  }
  .phonenum {
    float: right;
    font-size: 22px;
    line-height: 72px;
    font-family: "PingFangSC-Medium";
    font-weight: 600;
  }
  .catalog {
    display: none;
  }
}
@media screen and (min-width: 768px) and (max-width: 992px) {
  .header-nav {
    width: 100%;
    height: 72px;
    color: #1d2221;
    font-size: 16px;
    padding: 0 16px;
    box-sizing: border-box;
  }
  .header-nav a {
    color: #1d2221;
  }
  .header-nav-left {
    height: 100%;
    float: left;
    line-height: 72px;
  }
  .logo-container {
    display: block;
    width: 157px;
    height: 100%;
    display: flex;
    align-items: center;
    float: left;
  }
  .logo-container img {
    height: 44px;
  }
  .header-nav-right {
    height: 100%;
    float: right;
    display: flex;
    align-items: center;
  }
  .free-btn {
    width: 96px;
    height: 36px;
    background-color: #7bf8d8;
    border-radius: 20px;
    float: right;
    font-size: 16px;
    line-height: 36px;
    text-align: center;
  }
  .phonenum {
    display: none;
  }
  .line {
    display: none;
  }
  .catalog {
    display: none;
  }
}
@media screen and (max-width: 768px) {
  .header-nav {
    width: 100%;
    height: 72px;
    color: #1d2221;
    font-size: 16px;
    padding: 0 24px;
    box-sizing: border-box;
  }
  .header-nav a {
    color: #1d2221;
  }
  .header-nav-left {
    height: 100%;
    float: left;
    line-height: 72px;
  }
  .logo-container {
    display: block;
    width: 97px;
    height: 100%;
    display: flex;
    align-items: center;
    float: left;
  }
  .logo-container img {
    height: 44px;
  }
  .header-nav-item {
    display: none;
  }
  .header-nav-right {
    height: 100%;
    float: right;
    display: flex;
    align-items: center;
  }
  .free-btn {
    display: none;
  }
  .phonenum {
    float: right;
    font-size: 22px;
    line-height: 72px;
    font-family: "PingFangSC-Medium";
    font-weight: 600;
    display: none;
  }
  .line {
    display: none;
  }
  .catalogbtn {
    display: block;
  }
}
</style>