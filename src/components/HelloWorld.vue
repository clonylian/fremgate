<template>
  <div class="hello">
    <div class="head">
      <div class="head_one">
        <a href="">
          <img src="../assets/login.svg">
        </a>
        <div class="head_two">
          <a target="_blank"  href="https://www.frengate.app/connect">
            <div class="head_three">
              App (Launch Tonight)
              <img src="../assets/left.svg">
            </div>
          </a>
        </div>
      </div>
    </div>
    <div class="head_left">
      <div class="head_left2">
        <nav class="head_left3">
          <a href="#one">Hero</a>
          <a href="#two">Steps</a>
          <a href="#three">Features</a>
          <a href="#four">FAQ</a>
        </nav>
      </div>
    </div>
    <div class="cent">
      <div class="cent_1">
        <div class="cent_2" id="one">
          <div class="cent_3">
            <div class="cen_left">
              <h1>
                Your Shares,
                <span style="color: #00b3ef;">
                  Your Access
                </span>
              </h1>
              <div class="cent_4">
                We're empowering creators with simplified, secure, and transparent Discord &amp; Telegram authentication
                solutions. All built on a thriving community with a well researched and sustainable ecosystem.
              </div>
              <div class="cent_5">
                <a target="_blank" >
                  <div @click="add" class="head_three">
                        Connect
                    <img src="../assets/left.svg">
                  </div>
                </a>
                <div class="cent_6">
                  <a target="_blank" href="https://twitter.com/frengate">
                    <p>Twitter</p>
                    <img src="../assets/twitter.svg">
                  </a>
                </div>
              </div>
            </div>
            <div class="cent_right">
              <img src="../assets/1.png">
            </div>
          </div>
        </div>
      </div>
      <div class="container" :class="{ 'white-background': isScrolled }">
        <div class="bai">
          <div class="bai_1" id="two">
            <div class="bai_3">
              <h1>Buy</h1>
              <p>Powerful, self-serve product and growth analytics to help you convert, engage, and retain more.</p>
            </div>
            <div class="bai_3">
              <h1>Burn</h1>
              <p>Some of our tokens are heading to the bonfire to keep things lean! Less supply, more demand—simple as that.</p>
            </div>
            <div class="bai_3">
              <h1>Share</h1>
              <p>Share your frengate profile with the community and start connecting! Frens are deeper than just tokens.</p>
            </div>
          </div>
          <div class="bai_2">
            <img src="../assets/2.png">
          </div>
        </div>
      </div>
      <div class="feat" :class="{ 'white-background': isScrolled }">
        <h1 id="three">Features</h1>
        <div class="feat_1">
          <div class="feat_2">
            <img src="../assets/5.png">
            <div class="feat_3">
              <h2>Only shareholders gain access</h2>
              <p>Tired of manually adding and verifying new shareholders? frengate does this automatically, 24/7</p>
            </div>
          </div>
          <div class="feat_2">
            <img src="../assets/6.png">
            <div class="feat_3">
              <h2>Find your community</h2>
              <p>Search for new communities based on interest, find new users, or join your existing frens.</p>
            </div>
          </div>
          <div class="feat_2">
            <img src="../assets/7.png">
            <div class="feat_3">
              <h2>No security risks</h2>
              <p>frengate requires zero smart contract interaction, ensuring your wallets stay secure and your funds are
                safu.</p>
            </div>
          </div>
          <div class="feat_2">
            <img src="../assets/8.png">
            <div class="feat_3">
              <h2>User and Creator pages</h2>
              <p>Add some flair to your pages with group descriptions, interest tabs, analytics, and more!</p>
            </div>
          </div>
          <div class="feat_2">
            <img src="../assets/9.png">
            <div class="feat_3">
              <h2>1 minute to setup</h2>
              <p>Link your Discord / Telegram community to your Friend Tech account in less than a minute. It's that easy.
              </p>
            </div>
          </div>
          <div class="feat_2">
            <img src="../assets/10.png">
            <div class="feat_3">
              <h2>Only shareholders gain access</h2>
              <p>Tired of manually adding and verifying new shareholders? frengate does this automatically, 24/7</p>
            </div>
          </div>
        </div>
      </div>
      <div class="frens">
        <h2>
          <spa style=" color: #00b3ef;">frens,</spa>
          <br>
          ‍deeper than just coins.
        </h2>
        <div class="frens_1">
          <img src="../assets/23.png">
        </div>
      </div>
      <div class="asked" id="four">
        <h1>‍Frequently Asked Questions</h1>
      </div>
      <div class="asked_1">
        <div @click="changeTab('tab1')" :class="{ active: activeTab === 'tab1' }">About Us</div>
        <div @click="changeTab('tab2')" :class="{ active: activeTab === 'tab2' }">Authentication</div>
        <div @click="changeTab('tab3')" :class="{ active: activeTab === 'tab3' }">Rewards</div>
      </div>
      <div class="asked_2" v-show="activeTab === 'tab1'">
        <div class="asked_3">
          <div class="asked_4">
            <h2>What is frengate's primary goal?</h2>
            <img src="../assets/tt.svg">
          </div>
          <p>rengate aims to bridge gaps in the friend tech ecosystem by simplifying the creation and management of
            Discord and Telegram communities while ensuring secure key holder authentication.</p>
        </div>
        <div class="asked_3">
          <div class="asked_4">
            <h2>Is frengate a paid service?</h2>
            <img src="../assets/tt.svg">
          </div>
          <p>frengate's authentication and loyalty rewards calculator are paid services. all data analytics and dashboards
            on our sites are free to use for everyone</p>
        </div>
        <div class="asked_3">
          <div class="asked_4">
            <h2>How does frengate help creators?</h2>
            <img src="../assets/tt.svg">
          </div>
          <p>frengate enables creators to establish and manage communities effortlessly, complete with automatic key
            holder authentication. frengate also helps creators to rank their loyal keyholders, and calculate how much %
            of rewards each keyholder should receive. this is especially useful for communities that act as a farm</p>
        </div>
        <div class="asked_3">
          <div class="asked_4">
            <h2>How does frengate help key holders?</h2>
            <img src="../assets/tt.svg">
          </div>
          <p>stay tuned to our twitter... there is much more than rewards distribution</p>
        </div>
        <div class="asked_3">
          <div class="asked_4">
            <h2>Do I need to interact with any smart contracts?</h2>
            <img src="../assets/tt.svg">
          </div>
          <p>The only smart contract interaction required is when a creator swaps to buy our $FGATE token, which can be
            done either on UniSwap or on our site.</p>
        </div>
      </div>
      <div class="asked_2" v-show="activeTab === 'tab2'">
        <div class="asked_3">
          <div class="asked_4">
            <h2>Are there customizability options for the mininum number of keys required?</h2>
            <img src="../assets/tt.svg">
          </div>
          <p>Yes, you have full control to set the minimum number of keys required for individuals to access your
            community.</p>
        </div>
        <div class="asked_3">
          <div class="asked_4">
            <h2>How do users verify their key holder status?</h2>
            <img src="../assets/tt.svg">
          </div>
          <p>Users can easily verify their key holder status without any smart contract interaction. All they need to do
            is sign to verify the ownership of their wallet.</p>
        </div>
      </div>
      <div class="asked_2" v-show="activeTab === 'tab3'">
        <div class="asked_3">
          <div class="asked_4">
            <h2>What does the frengate Loyalty Rewards Calculator do?</h2>
            <img src="../assets/tt.svg">
          </div>
          <p>frengate's Loyalty Rewards Calculator allows creators to easily calculate who their loyal holders are without
            any risk of getting exploited or "gamed" by whales</p>
        </div>
        <div class="asked_3">
          <div class="asked_4">
            <h2>How does frengate prevent exploitation in rewards distribution?</h2>
            <img src="../assets/tt.svg">
          </div>
          <p>frengate rewards calculation system takes into account factors like key accumulation by whales and wash
            trading to ensure fair rewards for everyone.</p>
        </div>
      </div>
      <div class="build">
        <img src="../assets/17.png">
        <div class="bulid_1">
          <h1>Build or join a community, today.</h1>
          <p>We empower friend.tech creators to build stronger & safer communities with ease while also rewarding their
            shareholders.</p>
          <div class="bulid_2">
            <a href="https://www.frengate.app/connect">
              <div class="bulid_3">
                Access App
                <img src="../assets/right.svg">
              </div>
            </a>
            <a href="https://twitter.com/frengate">
              <div class="bulid_4">
                Twitter
                <img src="../assets/twitter.svg">
              </div>
            </a>
          </div>
        </div>
      </div>
      <div class="button">
        <img src="../assets/login.svg">
        <div class="button_1">
          <p><a href="#">Home</a></p>
          <p><a href="https://www.frengate.app/connect">App (Launch Tonight)</a></p>
          <p><a href="https://www.frengate.app/tokenomics">Tokenomics</a></p>
        </div>
        <div class="button_2">
          <p>© 2023 Frengate. All rights reserved.</p>
          <div class="button_3">
            <p class="button_4"><a href="https://www.frengate.app/privacy">Privacy Policy</a> </p>
            <p><a href="https://twitter.com/filter"> Designed by Filter® Studio</a></p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data() {
    return {
      isScrolled: false,
      activeTab: 'tab1',
    }
  },
  mounted() {
    window.addEventListener('scroll', this.handleScroll);
  },
  beforeDestroy() {
    window.removeEventListener('scroll', this.handleScroll);
  },
  methods: {
    handleScroll() {
      const scrollPosition = window.scrollY || document.documentElement.scrollTop;
      if (scrollPosition >= 700) {
        this.isScrolled = true; // 滚动到距离顶部 500px 处时，将 isScrolled 设置为 true
      } else {
        this.isScrolled = false; // 否则将 isScrolled 设置为 false
      }
    },
    changeTab(tab) {
      this.activeTab = tab;
    },
    add(){
      main();
    }

  },

}
</script>
<style scoped lang="scss">
@font-face {
  font-family: 'one';
  src: url('../assets/one.woff2') format('woff2'),
}

@font-face {
  font-family: 'two';
  src: url('../assets/two.otf') format('woff2'),
}

@font-face {
  font-family: 'three';
  src: url('../assets/three.ttf') format('woff2'),
}

.head {
  min-height: 5rem;
  -webkit-backdrop-filter: blur(14px);
  backdrop-filter: blur(14px);
  background-color: rgba(9, 9, 15, .03);
  border-bottom: 1px #f2f4f7;
  align-items: center;
  padding-left: 2rem;
  // padding-right: 2rem;
  display: flex;
  position: -webkit-sticky;
  position: sticky;
  top: 0;
  z-index: 3;
}

.head_one {
  width: 100%;
  height: 100%;
  max-width: 89rem;
  justify-content: flex-start;
  align-items: center;
  margin-left: auto;
  margin-right: auto;
  display: flex;
  justify-content: space-between
}

.head_one>a>img {
  width: 131px;
  height: 32px;
}

.head_two>a {
  grid-column-gap: 12px;
  grid-row-gap: 12px;
  color: white;
  color: rgba(255, 255, 255, .64);
  background-color: #00b3ef;
  border-radius: 10px;
  justify-content: center;
  align-items: center;
  padding: 9px 18px;
  font-size: .85rem;
  font-weight: 500;
  text-decoration: none;
  transition: all .2s;
  display: flex;
  font-family: one;
  box-shadow: 0 10px 30px rgba(43, 180, 239, .51);
}

.head_three {
  display: flex;
  align-items: center
}
.head_two>a:hover{
  background-color: #177dc6;
}
.head_three>img {
  width: 20px;
  height: 24px;
  margin-left: 1rem;
}

.head_left {
  width: 150px;
  height: 100%;
  mix-blend-mode: difference;
  background-color: rgba(0, 0, 0, 0);
  display: flex;
  position: fixed;
  top: 0%;
  bottom: 0%;
  left: auto;
  right: 0%;
  z-index: 2;
}

.head_left1 {
  margin-left: auto;
  margin-right: auto;
  max-width: 940px
}

.head_left2 {
  margin-left: auto;
  margin-right: auto;
  max-width: 940px;
}

.head_left3 {
  width: 100%;
  height: 100%;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  display: flex;
  position: relative;
  float: right;
}

.head_left3>a {

  max-width: 940px;
  color: #fff;
  background-color: rgba(0, 0, 0, 0);
  width: 100%;
  color: rgba(255, 255, 255, .21);
  text-align: center;
  background-color: rgba(0, 0, 0, 0);
  font-family: one;
  font-size: 18px;
  font-weight: 500;
  transition: all .2s;
  display: flex;
  color: white;
  padding: 1rem 0 1rem 0;
}

.cent {
  width: 100%;
  // padding-left: 2rem;
  // padding-right: 2rem;
  overflow: hidden;
  box-sizing: border-box;
}

.cent_1 {
  width: 100%;
  max-width: 80rem;
  margin-left: auto;
  margin-right: auto;
}

.cent_2 {
  padding-top: 10rem;
  padding-bottom: 7rem;
}

.cent_3 {
  grid-column-gap: 4rem;
  grid-row-gap: 4rem;
  grid-template-rows: auto;
  grid-template-columns: 1fr 1fr;
  grid-auto-columns: 1fr;
  align-items: center;
  display: grid;
}

.cen_left {
  padding-right: 52px;
}

.cen_left>h1 {
  color: #fcfcfc;
  margin-top: 0;
  margin-bottom: 0;
  font-size: 3.5rem;
  font-weight: 500;
  line-height: 1.1;
  font-family: one;
}

.cent_4 {
  color: #4f4f53;
  text-align: center;
  font-size: 1rem;
  font-weight: 500;
  line-height: 1.5;
  text-align: left;
  margin-top: 1.5rem;
  font-family: three;
  margin-bottom: 1.5rem;
}

.cent_5 {
  display: flex;
  align-items: center
}

.cent_5>a {
  grid-column-gap: 12px;
  grid-row-gap: 12px;
  color: white;
  color: rgba(255, 255, 255, .64);
  background-color: #00b3ef;
  border-radius: 10px;
  justify-content: center;
  align-items: center;
  padding: 9px 18px;
  font-size: 0.85rem;
  font-weight: 500;
  text-decoration: none;
  transition: all 0.2s;
  display: flex;
  font-family: one;
  box-shadow: 0 10px 30px rgba(43, 180, 239, .51);
}

.cent_5>a:hover {
  background-color: #177dc6;
}

.cent_6 {
  width: 8rem;
  height: 3rem;
  background-color: #1c1c22;
  border-radius: 10px;
  justify-content: center;
  align-items: center;
  // padding: 9px 18px;
  font-size: 0.85rem;
  font-weight: 500;
  text-decoration: none;
  transition: all 0.2s;
  display: flex;
  font-family: one;
  margin-left: 1rem;
}

.cent_6:hover {
  background-color: #2c2c35;
}

.cent_6>a {
  display: flex;
  align-items: center
}

.cent_6>a>p {
  color: white;
}

.cent_6>a>img {
  width: 20px;
  height: 24px;
  margin-left: 1rem;
  // background-color: #2c2c35;
}

.cent_right {
  height: 100%;
  min-height: 44rem;
  position: relative;


}

.cent_right>img {
  width: 71rem;
  min-width: 71rem;
  display: block;
  position: absolute;
  max-width: 100%;
  vertical-align: middle;
  height: auto;
  width: 100%;
}

.container {
  transition: background-color 1s ease-out;
  background-color: #000;
  /* 默认背景颜色 */
  display: flex;
  justify-content: center;
  padding-top: 10rem;
  padding-bottom: 15rem;
}

.white-background {
  background-color: white;
  /* 切换到的白色背景颜色 */
}

.bai {
  max-width: 100rem;
  width: 80%;
  display: flex;
  // margin: 0 auto;
  justify-content: space-between;
  align-items: center;
}

.bai_1 {
  width: 50%;
  // display: flex;
}

.bai_1 {
  display: flex;
  flex-direction: column;
}

.bai_2 {
  width: 50%;
  display: flex;
  justify-content: center;
}

.bai_2>img {
  border: 1px rgba(0, 0, 0, 0.57) solid;
  border-radius: 15px;
}

.bai_3 {
  width: 80%;
  margin-bottom: 2rem;
  font-family: three;
}

.bai_3>h1 {
  font-size: 2.5rem;
}

.bai_3>p {
  color: rgba(0, 0, 0, 0.57);
  font-size: 1.1rem;
  font-weight: 500;
  line-height: 1.5rem;
  margin-top: 1.5rem;
}

.feat {
  // height: 2000px;
  width: 100%;
  padding-bottom: 10rem;
}

.feat>h1 {
  color: #00b3ef;
  font-family: three;
  font-size: 60px;
  font-weight: 500;
  text-align: center;
  margin-bottom: 10rem;

}

.feat_1 {
  width: 80%;
  display: flex;
  margin: 0 auto;
  flex-wrap: wrap;
  justify-content: space-between;
}

.feat_2 {
  max-width: 450px;
  width: 32%;
  border: 1px #e8e8e8 solid;
  border-radius: 15px;
  margin-bottom: 2rem;
}

.feat_2:hover {
  transform: scale(0.98);
}

.feat_2>img {
  max-width: 100%;
  vertical-align: middle;
  display: inline-block;
  border-radius: 15px;
}

.feat_3 {
  padding: 1rem 1rem 3rem 1rem;
}

.feat_3>h2 {
  margin-bottom: 1rem;
}

.frens {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding-bottom: 20rem;
}

.frens>h2 {
  padding-top: 50rem;
  color: white;
  text-align: center;
  font-size: 35px;
  font-family: one;
  font-weight: 700;
  margin-bottom: 20rem;
}

.frens_1>img {
  width: 800px;
  // height: 650px;
}

.asked {
  width: 100%;
  padding-top: 15rem;
}

.asked>h1 {
  color: white;
  font-weight: 600;
  font-family: one;
  text-align: center;
  margin-bottom: 5rem;
}

.asked_1 {
  width: 50%;
  margin: 0 auto;
  color: white;
  display: flex;
  justify-content: center;
  padding-bottom: 5rem;
}

.asked_1>div:hover {
  height: 100%;
  color: #00b3ef;
  background-color: rgba(0, 179, 240, .24);
  border-style: none;
  border-radius: 40px;
  justify-content: center;
  align-items: center;
  margin-left: 0;
  margin-right: 0;
  font-weight: 500;
  display: flex;
  color: rgb(229, 231, 235);
  margin-left: 2rem;
}

.asked_1>div {
  margin-left: 2rem;
  padding: 0rem 1rem 0rem 1rem;
  border-radius: 30px;
  // background-color:#00b3ef ;
  text-align: center;
  line-height: 3rem;
}

.asked_2 {
  width: 50%;
  margin: 0 auto;
  color: white;
  font-family: one;
  display: flex;
  justify-content: center;
  justify-content: center;
  flex-direction: column;
  align-items: center;
  margin-bottom: 5rem;
}

.asked_3 {
  width: 80%;
  display: flex;
  flex-direction: column;
  border-bottom: 1px #4f4f53 solid;
  margin-bottom: 1rem;
}

.asked_3:hover {
  // transform: scale(0.96);
  padding-left: 10px;
}

.asked_4 {
  display: flex;
  justify-content: space-between;
}

.asked_4>h2 {
  font-size: 20px;
  font-family: one;
  font-weight: 500;
  margin-bottom: 1.5rem;
}

.asked_4>img {
  width: 20px;
  height: 20px;
}

.asked_3>p {
  max-width: 90%;
  color: #4f4f53;
  padding-bottom: 1.5rem;
  font-size: 0.9rem;
  font-weight: 500;
  font-family: one;
}

.build {
  width: 60%;
  margin: 0 auto;
  // height: 60rem;
  background-color: #00b3ef;
  background-image: linear-gradient(rgba(0, 179, 239, .73), rgba(0, 179, 239, .73)), url('../assets/19.png');
  background-position: 0 0, 50% 100%;
  background-repeat: repeat, no-repeat;
  background-size: auto, auto;
  border: 1px solid rgba(255, 255, 255, 0.14);
  border-radius: 20px;
  box-shadow: 0 0 60px -1px rgba(0, 179, 239, 0.18);
  display: flex;
  flex-direction: column;
  align-items: center;
}

.build>img {
  width: 767px;
  height: 320px;
  margin-top: 5rem;
}

.bulid_1 {
  width: 100%;
  max-width: 48rem;
  flex-direction: column;
  align-items: center;
  display: flex;
  text-align: center;
  color: white;
  font-family: one;
}

.bulid_1>h1 {
  font-size: 50px;
  margin-top: 1rem;
  margin-bottom: 1rem;
}

.bulid_1>p {
  color: rgba(255, 255, 255, .71);
  font-weight: 500;
  margin-bottom: 2rem
}

.bulid_2 {
  width: 100%;
  display: flex;
  justify-content: center;
  padding-bottom: 5rem;
  align-items: center
}

.bulid_3 {
  padding: 0.8rem 1rem 0.8rem 1rem;
  background-color: white;
  color: rgba(0, 138, 183, 0.47);
  display: flex;
  border-radius: 5px;
  margin-right: 1rem;
  font-size: 14px;
}

.bulid_3>img {
  width: 15px;
  height: 15px;
  margin-left: 1rem;
}

.bulid_4 {
  padding: 0.6rem 1rem 0.6rem 1rem;
  background-color: #000;
  color: white;
  // color: rgba(0, 138, 183, 0.47);
  display: flex;
  font-weight: 600;
  border-radius: 5px;
  align-items: center
}

.bulid_4>img {
  width: 20px;
  height: 20px;
  margin-left: 1rem;
}

.button {
  width: 80%;
  margin: 0 auto;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.button>img {
  width: 107px;
  height: 32px;
  margin-top: 8rem;
}

.button_1 {
  width: 100%;
  color: white;
  display: flex;
  justify-content: center;
  margin: 3rem 0 1.5rem 0;
  padding-bottom: 5rem;
  border-bottom: 1px #e5e7eb solid;
}

.button_1>p>a {
  margin-right: 2rem;
  color: #7b7b7b;
}

.button_1>p>a:hover {
  color: white;
}

.button_1>p>a:nth-child(2) {
  color: rgba(229, 231, 235, 0.5);
}

.button_2 {
  width: 100%;
  margin: 0 auto;
  padding-bottom: 2rem;
  color: #7b7b7b;
  display: flex;
  justify-content: space-between;
}

.button_3 {
  display: flex;
}

.button_3>p>a {
  color: #7b7b7b;
}

.button_3>p>.asked_3:hover {
  color: white;
}
.button_2>p:hover{
    color: #d7d7d7;
}
.button_4 {
  margin-right: 1rem;
}
.button_3>p>a:hover{
  color: #d7d7d7;
}

@media (max-width: 600px) {
  .head_left {
    display: none;
  }

  .head {
    padding-left: 0;
  }

  .head_one {
    max-width: 9rem;
  }

  .head_two {
    display: none;
  }

  .cent_1 {}

  .cent_2 {
    padding-top: 0;
  }

  .cen_left {
    padding-right: 0;
  }

  .cent_3 {
    display: block;
  }

  .cent_5 {
    display: block;

  }
  .feat_3{
    padding: 1rem 1rem 2rem 1rem;
  }
  .cent_6 {
    width: 100%;
    margin-left: 0;
    margin-top: 1rem;
  }

  .cent_right {
    display: flex;
    min-height: 0rem;
    justify-content: center;
  }

  .cent_right>img {
    width: 343px;
    height: 191px;
   min-width: 22rem;
  }

  .container {
    // padding-top: 0rem;
  }

  .bai {
    flex-direction: column;
    width: 100%;
  }

  .bai_1 {
    width: 90%;
  }

  .bai_2 {
    width: 100%;
  }

  .bai_2>img {
    width: 90%;
  }

  .feat_1 {
    flex-direction: column;
  }

  .feat_2 {
    width: 100%;
  }

  .frens {
    display: none;
  }

  .asked {
    padding-top: 5rem;
  }

  .asked_1 {
    text-align: center;
    flex-direction: column;
    align-items: center;
  }

  .asked_1>div {
    margin-left: 0rem;
  }

  .asked_1>div:hover {
    margin-left: 0rem;
  }

  .asked_2 {
    width: 99%;
  }

  .build {
    width: 90%;
  }

  .build>img {
    width: 314px;
    height: 130px;
  }

  .bulid_1>h1 {
    font-size: 40px;
  }

  .bulid_2 {
    flex-direction: column;
    align-items: normal;
    padding-bottom: 2rem;
  }

  .bulid_3 {
    margin-right: 0rem;
    margin-bottom: 1rem;
    justify-content: center;
  }

  .bulid_4 {
    justify-content: center;
  }

  .button {
    width: 100%;
  }

  .button_1 {
    justify-content: space-around;
  }

  .button_1>p>a {
    margin-right: 0rem;
  }
  .button_2{
    flex-direction: column;
    align-items: center;
  }
}</style>

