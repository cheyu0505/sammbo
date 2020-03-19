<template>
  <div class="index">
    <div class="content">
      <div class="background1">
        <div class="intro">
          <div class="intro-left">
            <div class="intro-left-title">闪布 高效工作成就自由生活</div>
            <p class="intro-left-detail hidden2">一触即达的沟通方式、一目了然的工作计划、一诺千金的安全保障，尽在闪布。</p>
            <div class="intro-free-btn">免费使用</div>
          </div>
          <div class="intro-right">
            <img src="../assets/img/01 01@3x.png" alt="加载失败" />
          </div>
        </div>
        <p class="middle-title">轻松点亮职场关系网</p>
        <div class="message">
          <div class="message-right">
            <p class="message-right-title">消息触达无障碍 历史消息群共享</p>
            <div class="message-right-detail">闪布未读消息及时通过短信邮件有效传递，打破沟通壁垒，群历史消息可选择对新群成员共享，快速同步重要信息。</div>
          </div>
          <div class="message-img">
            <img src="../assets/img/01 02@3x.png" alt="加载失败" />
          </div>
        </div>
      </div>

      <div class="operation">
        <div class="operation-left">
          <div class="operation-left-title">一条消息轻巧转换多重动作</div>
          <div class="operation-left-detail">
            “标记”——重要信息自动加粗
            <br />“引用回复”——群聊中的极致降噪利器
            <br />“转代办”——快捷指派紧急任务
          </div>
          <div class="detail-btn detail">了解详情</div>
        </div>
        <div class="operation-img">
          <img src="../assets/img/01 04@3x.png" alt="加载失败" />
        </div>
      </div>
      <div class="mutualtrust">
        <div class="mutualtrust-left">
          <div class="mutualtrust-left-title">闪布独有企业互信 让合作更亲近</div>
          <div class="mutualtrust-left-detail">闪布企业互信对外展示信息可配置，让合作更亲密更放心。</div>
          <div class="detail-btn detail">了解详情</div>
        </div>
        <div class="mutualtrust-img">
          <img src="../assets/img/01 03@3x.png" alt="加载失败" />
        </div>
      </div>
      <div class="safeguard">
        <div class="safeguard-title">层层保障，为信息安全保驾护航</div>
        <div class="safeguard-box">
          <div class="safeguard-box-item">
            <img src="../assets/img/01_04icon_加密算法@2x.png" alt />
            <span>加密算法</span>
          </div>
          <div class="safeguard-box-item">
            <img src="../assets/img/01_04icon_安全审计@2x.png" alt />
            <span>安全审计</span>
          </div>
          <div class="safeguard-box-item">
            <img src="../assets/img/01_04icon_全量备份@2x.png" alt />
            <span>全量备份</span>
          </div>
          <div class="safeguard-box-item">
            <img src="../assets/img/01_04icon_持续稳定@2x.png" alt />
            <span>持续稳定</span>
          </div>
        </div>
        <div class="safeguard-box-item-box">
          <div class="safeguard-box-item">
            <img src="../assets/img/01_04icon_加密算法@2x.png" alt />
            <span>加密算法</span>
          </div>
          <div class="safeguard-box-item">
            <img src="../assets/img/01_04icon_安全审计@2x.png" alt />
            <span>安全审计</span>
          </div>
        </div>
        <div class="safeguard-box-item-box">
          <div class="safeguard-box-item">
            <img src="../assets/img/01_04icon_全量备份@2x.png" alt />
            <span>全量备份</span>
          </div>
          <div class="safeguard-box-item">
            <img src="../assets/img/01_04icon_持续稳定@2x.png" alt />
            <span>持续稳定</span>
          </div>
        </div>
      </div>
      <div class="middle-title" style="margin-bottom: 18px">众多企业的信赖之选</div>
      <div class="smalltitle">闪布致力于为企业提供安全高效的协同办公新方式</div>
      <div class="cardbox">
        <div class="carditem">
          <div class="imgbox img1">
            <img src="../assets/img/01 05_1@2x.jpg" alt />
          </div>
          <div class="cardtext">
            <p>互联网/信息技术</p>
            <p>契合年轻群体，让管理更有温度</p>
          </div>
        </div>
        <div class="carditem">
          <div class="imgbox img2">
            <img src="../assets/img/01 05_2@2x.jpg" alt />
          </div>
          <div class="cardtext">
            <p>制造业/新零售</p>
            <p>闪布加固核心凝聚力，不断提升营业额</p>
          </div>
        </div>
        <div class="carditem">
          <div class="imgbox img3">
            <img src="../assets/img/01 05_3@2x.jpg" alt />
          </div>
          <div class="cardtext">
            <p class="hidden1">供应链/外包服务业</p>
            <p class="hidden2">群话题、群投票等多功能支持，带来透明、平等、温暖的企业管理文化。</p>
          </div>
        </div>
      </div>
    </div>
    <div class="bottomtext">
      <div class="middle-title" style="margin-bottom: 18px">众多企业的信赖之选</div>
      <div class="smalltitle">闪布致力于为企业提供安全高效的协同办公新方式</div>
      <div class="btn">
        <div class="freebtn free">免费使用</div>
        <div class="detail-btn free">联系我们</div>
      </div>
    </div>
    <footerbox></footerbox>
  </div>
</template>

<script>
import morelistitem from "../components/morelistitem";
import morelistitem1 from "../components/morelistitem1";
import footerbox from "../components/footer";
export default {
  name: "Index",
  data() {
    return {
    };
  },
  components: {
    morelistitem,
    morelistitem1,
    footerbox
  },
  mounted() {},
};
</script>
<style>
.qr {
  width: 72px;
  height: 72px;
}
.index {
  margin-top: 72px;
}
.intro {
  width: 100%;
  height: 500px;
}
.middle-title {
  font-family: "PingFangSC-Semibold";
  font-size: 36px;
  color: #1d2221;
  text-align: center;
  line-height: 44px;
  margin-top: 80px;
  margin-bottom: 36px;
  font-weight: 600 !important;
}
.smalltitle {
  font-family: "PingFangSC-Regular";
  font-size: 16px;
  color: #6c6f6e;
  text-align: center;
  line-height: 24px;
  text-align: center;
}
.safeguard {
  width: 100%;
  height: 500px;
  padding-top: 80px;
  box-sizing: border-box;
}
.safeguard-title {
  font-family: "PingFangSC-Semibold";
  font-size: 36px;
  color: #1d2221;
  text-align: center;
  line-height: 44px;
  font-weight: 600;
}
.safeguard-box {
  width: 100%;
  margin-top: 98px;
  display: flex;
  justify-content: space-around;
  flex-wrap: wrap;
}
.safeguard-box-item {
  width: 128px;
  text-align: center;
}
.safeguard-box-item img {
  width: 100%;
  margin-bottom: 42px;
}
.safeguard-box-item span {
  font-family: "PingFangSC-Medium";
  font-size: 20px;
  color: #1d2221;
  line-height: 28px;
  font-weight: 600;
}
.safeguard-box-item-box {
  display: none;
}
.cardbox {
  width: 100%;
  margin-top: 60px;
  display: flex;
  justify-content: space-between;
  margin-bottom: 104px;
}
.carditem {
  width: 352px;
}
.cardtext {
  width: 100%;
  padding: 0 24px;
  padding-bottom: 48px;
  box-sizing: border-box;
  overflow: hidden;
  box-shadow: 4px 4px #f5f5f5;
}
.cardtext :nth-child(1) {
  font-family: "PingFangSC-Medium";
  font-size: 20px;
  color: #1d2221;
  line-height: 28px;
  font-weight: 600;
  margin-top: 24px;
  margin-bottom: 12px;
}
.cardtext :nth-child(2) {
  font-family: "PingFangSC-Regular";
  font-size: 16px;
  color: #6c6f6e;
  line-height: 28px;
  height: 58px;
}
.carditem img {
  width: 100%;
}
.bottomtext {
  width: 100%;
  height: 339.7px;
  overflow: hidden;
  background-image: url("../assets/img/01 06.png");
}
.btn {
  margin-top: 59px;
  display: flex;
  justify-content: center;
}
.freebtn {
  background: #7bf8d8;
  border-radius: 20px;
}
.free {
  width: 128px;
  height: 40px;
  margin: 0 8px;
  box-sizing: border-box;
  line-height: 40px;
  text-align: center;
}
.detail-btn {
  width: 128px;
  height: 40px;
  border: 2px solid #7bf8d8;
  border-radius: 20px;
  text-align: center;
  line-height: 40px;
  font-family: "PingFangSC-Regular";
  font-size: 16px;
  color: #1d2221;
  box-sizing: border-box;
}
.detail {
  margin: 0 auto;
}
/* .background1{
  background-image: url("../assets/img/");
} */

@media screen and (min-width: 1201px) {
  .content {
    width: 1136px;
    margin: 0 auto;
  }
  .intro-left {
    width: 556px;
    padding-top: 110px;
    box-sizing: border-box;
    float: left;
  }
  .intro-left-title {
    font-family: "PingFangSC-Semibold";
    font-size: 40px;
    color: #1d2221;
    letter-spacing: 0;
    line-height: 48px;
    font-weight: 600;
  }
  .intro-left-detail {
    width: 475px;
    font-family: "PingFangSC-Regular";
    font-size: 20px;
    color: #6c6f6e;
    letter-spacing: 0;
    line-height: 32px;
    margin-top: 28px;
    margin-bottom: 82px;
  }
  .intro-free-btn {
    width: 128px;
    height: 40px;
    background: #7bf8d8;
    border-radius: 22px;
    text-align: center;
    line-height: 40px;
    font-family: PingFangSC-Regular;
    font-size: 16px;
    color: #1d2221;
  }
  .intro-right {
    float: right;
    width: 580px;
    height: 500px;
  }
  .intro-right img {
    width: 100%;
    height: 100%;
  }
  .message {
    width: 100%;
    height: 600px;
  }
  .message-img {
    width: 672px;
    height: 100%;
    margin-right: 48px;
    float: left;
  }
  .message-img img {
    height: 100%;
  }
  .message-right {
    width: 416px;
    float: right;
    height: 100%;
    padding-top: 200px;
    box-sizing: border-box;
  }
  .message-right-title {
    font-family: "PingFangSC-Semibold";
    font-size: 28px;
    color: #1d2221;
    letter-spacing: 0;
    line-height: 36px;
    font-weight: 600;
    margin-bottom: 18px;
  }
  .message-right-detail {
    width: 100%;
    font-family: "PingFangSC-Regular";
    font-size: 16px;
    color: #6c6f6e;
    letter-spacing: 0;
    line-height: 28px;
  }
  .operation {
    width: 100%;
    height: 600px;
  }
  .operation-left {
    width: 416px;
    height: 100%;
    float: left;
    padding-top: 200px;
    box-sizing: border-box;
  }
  .operation-left-title {
    font-family: "PingFangSC-Semibold";
    font-size: 28px;
    color: #1d2221;
    line-height: 36px;
    font-weight: 600;
  }
  .operation-left-detail {
    font-family: "PingFangSC-Regular";
    font-size: 16px;
    color: #6c6f6e;
    line-height: 28px;
    margin-top: 18px;
    margin-bottom: 32px;
  }
  .operation-img {
    float: right;
    width: 620px;
    height: 600px;
  }
  .operation-img img {
    height: 100%;
  }
  .mutualtrust {
    width: 100%;
    height: 600px;
  }
  .mutualtrust-left {
    width: 416px;
    height: 100%;
    float: right;
    padding-top: 200px;
    box-sizing: border-box;
  }
  .mutualtrust-left-title {
    font-family: "PingFangSC-Semibold";
    font-size: 28px;
    color: #1d2221;
    line-height: 36px;
    font-weight: 600;
  }
  .mutualtrust-left-detail {
    font-family: "PingFangSC-Regular";
    font-size: 16px;
    color: #6c6f6e;
    line-height: 28px;
    margin-top: 18px;
    margin-bottom: 32px;
  }
  .mutualtrust-img {
    float: left;
    width: 620px;
    height: 600px;
  }
  .mutualtrust-img img {
    height: 100%;
  }
}
@media screen and (min-width: 992px) and (max-width: 1200px) {
  .content {
    width: 942px;
    margin: 0 auto;
  }
  .intro-left {
    width: 420px;
    padding-top: 110px;
    box-sizing: border-box;
    float: left;
  }
  .intro-left-title {
    width: 337px;
    height: 96px;
    font-family: "PingFangSC-Semibold";
    font-size: 40px;
    color: #1d2221;
    letter-spacing: 0;
    line-height: 48px;
    font-weight: 600;
  }
  .intro-left-detail {
    width: 393px;
    font-family: "PingFangSC-Regular";
    font-size: 20px;
    color: #6c6f6e;
    letter-spacing: 0;
    line-height: 32px;
    margin-top: 28px;
    margin-bottom: 34px;
  }
  .intro-free-btn {
    width: 128px;
    height: 40px;
    background: #7bf8d8;
    border-radius: 22px;
    text-align: center;
    line-height: 40px;
    font-family: PingFangSC-Regular;
    font-size: 16px;
    color: #1d2221;
  }
  .intro-right {
    float: right;
    width: 522px;
    height: 450px;
  }
  .intro-right img {
    width: 100%;
    height: 100%;
  }
  .message {
    width: 100%;
    height: 600px;
  }
  .message-img {
    width: 537.6px;
    height: 480px;
    margin-top: 60px;
    float: left;
  }
  .message-img img {
    height: 100%;
  }
  .message-right {
    width: 366px;
    float: right;
    height: 100%;
    padding-top: 140px;
    box-sizing: border-box;
  }
  .message-right-title {
    font-family: "PingFangSC-Semibold";
    font-size: 28px;
    color: #1d2221;
    letter-spacing: 0;
    line-height: 36px;
    font-weight: 600;
    margin-bottom: 18px;
  }
  .message-right-detail {
    width: 100%;
    font-family: "PingFangSC-Regular";
    font-size: 16px;
    color: #6c6f6e;
    letter-spacing: 0;
    line-height: 28px;
  }
  .operation {
    width: 100%;
    height: 600px;
  }
  .operation-left {
    width: 366px;
    height: 100%;
    float: left;
    padding-top: 200px;
    box-sizing: border-box;
  }
  .operation-left-title {
    font-family: "PingFangSC-Semibold";
    font-size: 28px;
    color: #1d2221;
    line-height: 36px;
    font-weight: 600;
  }
  .operation-left-detail {
    font-family: "PingFangSC-Regular";
    font-size: 16px;
    color: #6c6f6e;
    line-height: 28px;
    margin-top: 18px;
    margin-bottom: 32px;
  }
  .operation-img {
    float: right;
    width: 537.6px;
    height: 480px;
    margin-top: 60px;
  }
  .operation-img img {
    height: 100%;
  }
  .mutualtrust {
    width: 100%;
    height: 600px;
  }
  .mutualtrust-left {
    width: 366px;
    height: 100%;
    float: right;
    padding-top: 200px;
    box-sizing: border-box;
  }
  .mutualtrust-left-title {
    font-family: "PingFangSC-Semibold";
    font-size: 28px;
    color: #1d2221;
    line-height: 36px;
    font-weight: 600;
  }
  .mutualtrust-left-detail {
    font-family: "PingFangSC-Regular";
    font-size: 16px;
    color: #6c6f6e;
    line-height: 28px;
    margin-top: 18px;
    margin-bottom: 32px;
  }
  .mutualtrust-img {
    float: left;
    width: 537.6px;
    height: 480px;
    margin-top: 60px;
  }
  .mutualtrust-img img {
    height: 100%;
  }
  .carditem {
    width: 240px;
  }
  .cardbox {
    justify-content: space-around;
  }
}
@media screen and (min-width: 768px) and (max-width: 992px) {
  .content {
    width: 100%;
    margin: 0 auto;
    padding: 0 16px;
    box-sizing: border-box;
  }
  .intro-left {
    width: calc(100% - 441px);
    padding-top: 110px;
    box-sizing: border-box;
    float: left;
  }
  .intro-left-title {
    width: 100%;
    height: 96px;
    font-family: "PingFangSC-Semibold";
    font-size: 40px;
    color: #1d2221;
    letter-spacing: 0;
    line-height: 48px;
    font-weight: 600;
  }
  .intro-left-detail {
    width: 100%;
    font-family: "PingFangSC-Regular";
    font-size: 20px;
    color: #6c6f6e;
    letter-spacing: 0;
    line-height: 32px;
    margin-top: 28px;
    margin-bottom: 34px;
  }
  .intro-free-btn {
    width: 128px;
    height: 40px;
    background: #7bf8d8;
    border-radius: 22px;
    text-align: center;
    line-height: 40px;
    font-family: PingFangSC-Regular;
    font-size: 16px;
    color: #1d2221;
  }
  .intro-right {
    float: right;
    height: 380px;
    margin-top: 40px;
  }
  .intro-right img {
    /* width: 100%; */
    height: 100%;
  }
  .message {
    width: 100%;
    height: 600px;
  }
  .message-img {
    height: 336px;
    margin-top: 60px;
    float: left;
  }
  .message-img img {
    height: 100%;
  }
  .message-right {
    width: 350px;
    float: right;
    height: 100%;
    padding-top: 140px;
    box-sizing: border-box;
  }
  .message-right-title {
    font-family: "PingFangSC-Semibold";
    font-size: 28px;
    color: #1d2221;
    letter-spacing: 0;
    line-height: 36px;
    font-weight: 600;
    margin-bottom: 18px;
  }
  .message-right-detail {
    width: 100%;
    font-family: "PingFangSC-Regular";
    font-size: 16px;
    color: #6c6f6e;
    letter-spacing: 0;
    line-height: 28px;
  }
  .operation {
    width: 100%;
    height: 600px;
  }
  .operation-left {
    width: 304px;
    height: 100%;
    float: left;
    padding-top: 200px;
    box-sizing: border-box;
  }
  .operation-left-title {
    width: 100%;
    font-family: "PingFangSC-Semibold";
    font-size: 28px;
    color: #1d2221;
    line-height: 36px;
    font-weight: 600;
  }
  .operation-left-detail {
    font-family: "PingFangSC-Regular";
    font-size: 16px;
    color: #6c6f6e;
    line-height: 28px;
    margin-top: 18px;
    margin-bottom: 32px;
  }
  .operation-img {
    float: right;
    width: 430px;
    height: 384px;
    margin-top: 108px;
  }
  .operation-img img {
    height: 100%;
  }
  .mutualtrust {
    width: 100%;
    height: 600px;
  }
  .mutualtrust-left {
    width: 304px;
    height: 100%;
    float: right;
    padding-top: 200px;
    box-sizing: border-box;
  }
  .mutualtrust-left-title {
    width: 100%;
    font-family: "PingFangSC-Semibold";
    font-size: 28px;
    color: #1d2221;
    line-height: 36px;
    font-weight: 600;
  }
  .mutualtrust-left-detail {
    font-family: "PingFangSC-Regular";
    font-size: 16px;
    color: #6c6f6e;
    line-height: 28px;
    margin-top: 18px;
    margin-bottom: 32px;
  }
  .mutualtrust-img {
    float: left;
    width: 430px;
    height: 384px;
    margin-top: 108px;
  }
  .mutualtrust-img img {
    height: 100%;
  }
  .carditem {
    width: 200px;
  }
  .cardbox {
    justify-content: space-around;
  }
}
@media screen and (max-width: 768px) {
  .content {
    width: 100%;
    padding: 0 24px;
    box-sizing: border-box;
    margin: 0 auto;
  }
  .intro {
    width: 100%;
    height: 678px;
  }
  .intro-left {
    width: 100%;
    padding-top: 36px;
    box-sizing: border-box;
  }
  .intro-left-title {
    font-family: "PingFangSC-Semibold";
    font-size: 32px;
    color: #1d2221;
    letter-spacing: 0;
    line-height: 40px;
    font-weight: 600;
  }
  .intro-left-detail {
    width: 100%;
    font-family: "PingFangSC-Regular";
    font-size: 20px;
    color: #6c6f6e;
    letter-spacing: 0;
    line-height: 32px;
    margin-top: 28px;
    margin-bottom: 40px;
  }
  .intro-free-btn {
    width: 128px;
    height: 40px;
    background: #7bf8d8;
    border-radius: 22px;
    text-align: center;
    line-height: 40px;
    font-family: PingFangSC-Regular;
    font-size: 16px;
    color: #1d2221;
  }
  .intro-right {
    float: right;
    width: 100%;
  }
  .intro-right img {
    width: 100%;
  }
  .message-img {
    width: 100%;
    /* height: 403.2px; */
    margin-top: 19px;
  }
  .message-img img {
    width: 100%;
    /* height: 100%; */
  }
  .message-right {
    width: 100%;
    padding-top: 80px;
    box-sizing: border-box;
  }
  .message-right-title {
    font-family: "PingFangSC-Semibold";
    font-size: 28px;
    color: #1d2221;
    letter-spacing: 0;
    line-height: 36px;
    font-weight: 600;
    margin-bottom: 16px;
    text-align: center;
  }
  .message-right-detail {
    width: 100%;
    font-family: "PingFangSC-Regular";
    font-size: 16px;
    color: #6c6f6e;
    letter-spacing: 0;
    line-height: 28px;
    text-align: center;
  }
  .operation {
    margin-top: 40px;
    width: 100%;
    padding-top: 40px;
    box-sizing: border-box;
  }
  .operation-left-title {
    width: 100%;
    text-align: center;
    font-family: "PingFangSC-Semibold";
    font-size: 28px;
    color: #1d2221;
    line-height: 36px;
    font-weight: 600;
    margin-bottom: 16px;
  }
  .operation-left-detail {
    font-family: "PingFangSC-Regular";
    font-size: 16px;
    text-align: center;
    color: #6c6f6e;
    line-height: 28px;
    margin-top: 18px;
    margin-bottom: 16px;
  }
  .operation-img {
    width: 100%;
    /* height: 420px; */
  }
  .operation-img img {
    width: 100%;
    /* height: 100%; */
  }
  .mutualtrust {
    margin-top: 40px;
    width: 100%;
    padding-top: 40px;
    box-sizing: border-box;
  }
  .mutualtrust-left-title {
    width: 100%;
    text-align: center;
    font-family: "PingFangSC-Semibold";
    font-size: 28px;
    color: #1d2221;
    line-height: 36px;
    font-weight: 600;
    margin-bottom: 16px;
  }
  .mutualtrust-left-detail {
    font-family: "PingFangSC-Regular";
    font-size: 16px;
    text-align: center;
    color: #6c6f6e;
    line-height: 28px;
    margin-top: 18px;
    margin-bottom: 16px;
  }
  .mutualtrust-img {
    width: 100%;
    /* height: 420px; */
  }
  .mutualtrust-img img {
    width: 100%;
  }
  .safeguard {
    height: 680px;
  }
  .safeguard-box {
    display: none;
  }
  .safeguard-box-item-box {
    margin-top: 50px;
    display: block;
    width: 100%;
    display: flex;
    justify-content: space-around;
  }
  .carditem {
    width: 100%;
    margin-bottom: 40px;
  }
  .carditem img {
    display: none;
  }
  .carditem .imgbox {
    width: 100%;
    height: 380px;
    background-size: cover;
    background-repeat: no-repeat;
  }
  .carditem .img1 {
    background-image: url("../assets/img/01 05_1@2x.jpg");
  }
  .carditem .img2 {
    background-image: url("../assets/img/01 05_2@2x.jpg");
  }
  .carditem .img3 {
    background-image: url("../assets/img/01 05_3@2x.jpg");
  }
  .cardbox {
    display: block;
  }
}
</style>
