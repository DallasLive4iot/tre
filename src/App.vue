<template>
  <header class="start">
    <div v-bind:style="background">
      <div class="main body" style="height:640vh; background-repeat: no-repeat;">
        <div id="border" style="border:thick">
          <!-- <component-one children="For Shipper" style="background-color: aqua;"/> -->
          <div class="flex">
            <img src="@/assets/logo.png" style="height:fit-content; margin-top: 0; position: fixed; top:1vh ;" />
            <div class="flex3">
              <top-menu-button children="Overview" @click="handleClick" style="width:5" />
              <top-menu-button children="Services" @click="handleClick2" style="width:fit-content" />
              <top-menu-button children="Benefits" @click="handleClick3" style="width:fit-content" />
              <top-menu-button children="About Us" @click="handleClick4" style="width:fit-content" />
              <top-menu-button children="Contact Us" @click="handleClick5" style="width:fit-content" />

            </div>

          </div>
          <div class="Overview" style="position: absolute;top: 20vh; left: 10vw;" ref="Overview">
            <div class="main page" style="height: auto;width: auto;resize: both;">
              <h1 class="title2" style="margin-top: 1vh;">The Route Enterprise</h1>
              <h1 class="title3" style="text-align: center;">Join Us!</h1>
              <h1 class="title3" style="text-align: center;">Scan the QR code and download our App!</h1>
              <div class="flex2">
                <h1 class="title3">We provide</h1>
                <component-one children="integrated," style="background-color: #073E17AD;" />
                <component-one children="efficient," style="background-color: #073E17AD;" />
                <h1 class="title3">and</h1>
                <component-one children="cooperative" style="background-color: #073E17AD;" />
                <h1 class="title3">experience.</h1>
              </div>
            </div>



          </div>

        </div>
        <div class="ServicePage" style="position: absolute;top: 150vh;left: 5vw;" ref="Service">
          <h1
            style="position: absolute; top: 10vh; left: 5vw; font: italic normal bold 5vh Segoe UI;color: white;opacity: 1;">
            Services</h1>

          <green-box2-vue children="For Shipper"
            style="position: absolute; top: 25vh; left: 10vw;background-color: #e3f3e7;height: min-content;" />
          <green-box3-vue children="For Carrier" style="position: absolute; top: 55vh; left: 17vw;height: min-content;" />
          <green-box4-vue children="Tracking Device"
            style="position: absolute; top: 85vh; left: 24vw;height: min-content;" />
          <img src="@/assets/OBD.png" style="height:35vh; position: absolute; top: 92vh; left: 41vw;resize: both;" />
          <img src="@/assets/Screen1.png" style="height:65vh; position: absolute; top: 15vh; left: 55vw;resize: both;" />
          <img src="@/assets/Screen2.png" style="height:65vh; position: absolute; top: 45vh; left: 67vw;resize:both" />
          <img src="@/assets/running2.gif" style="height:20vh; position: absolute; top: 67vh; left: 61vw;resize: both;" />
        </div>
        <div class="Benefits Page" style="position: absolute;top: 20vh;">
          <h1 style="position:absolute;top:295vh" ref="Benefits"></h1>
          <h1
            style="position: absolute; top: 300vh; left: 5vw; font: italic normal bold 5vh Segoe UI;color: white;opacity: 1;">
            Benefits</h1>
          <h1 class="title3" style="position: absolute; top: 310vh;left: 5vw; width:45vw;">If you have ambitions, or want
            to get passive income? JOIN US AND BECOME OUR PARTNER! Download App check the benefits details!</h1>
          <img src="@/assets/infographic.png" style="height:60vh; position: absolute; top: 310vh; left: 40vw;resize: both;overflow: clip;" />
          <benefits-info style="position: absolute;top: 380vh;"></benefits-info>
        </div>
        <h1 style="position:absolute;top:415vh" ref="AboutUs"></h1>
        <div class="About us Page" style="position: absolute; top: 420vh; left: 5vw;">

          <h1 style=" font: italic normal bold 5vh Segoe UI;color: white;opacity: 1;">About Us</h1>
          <about-us-content-vue style="position: absolute; top: 30vh;left:5vw"></about-us-content-vue>
          <about-us-content-two-vue style="position: absolute; top: 30vh;left:35vw"></about-us-content-two-vue>
          <about-us-content-three-vue style="position: absolute; top: 30vh;left:65vw"></about-us-content-three-vue>
        </div>
        <div class="Join Us" style="position: absolute; top: 530vh; left: 5vw;">
          <h1 style=" font: italic normal bold 5vh Segoe UI;color: white;opacity: 1;" ref="Join">Join Us</h1>
          <scanneri-o-s-vue style="position: absolute;left: 0vw;top: 15vh;resize: both;"></scanneri-o-s-vue>
          <scanner-android-vue style="position: absolute;left: 20vw;top: 15vh;"></scanner-android-vue>
          <scanner-google-vue style="position: absolute;left: 40vw;top: 15vh;"></scanner-google-vue>
        </div>
        <div class="Contact Page" style="position: absolute; top: 600vh; left: 5vw;">
          <h1 style=" font: italic normal bold 5vh Segoe UI;color: white;opacity: 1;" ref="Contact">Contact Us</h1>
          <img src="@/assets/MapPin.png" style="height:3.5vh; position: absolute; top: 12vh; left: 0vw;" />
          <img src="@/assets/Phone.png" style="height:2.7vh; position: absolute; top: 17vh; left: 0vw;" />
          <img src="@/assets/Mail.png" style="height:1.9vh; position: absolute; top: 22vh; left: 0vw;" />
          <img src="@/assets/Terms.png" style="height:3vh; position: absolute; top: 27vh; left: 0vw;" />
          <img src="@/assets/Lock.png" style="height:3.1vh; position: absolute; top: 32vh; left: 0vw;" />
          <img src="@/assets/running3.gif"
            style="height:90vh;width: 47vw; position: absolute; top: -45vh; left: 47vw;resize: both;overflow: clip;" />

        </div>

      </div>
    </div>

  </header>
</template>

<script>

import ComponentOne from './components/ComponentOne.vue';
import TopMenuButton from '@/components/RedirectButton.vue'
import GreenBox2Vue from './components/GreenBox2.vue';
import GreenBox3Vue from './components/GreenBox3.vue';
import GreenBox4Vue from './components/GreenBox4.vue';
import BenefitsInfo from './components/BenefitsInfo.vue';
import AboutUsContentVue from './components/AboutUsContent.vue';
import AboutUsContentTwoVue from './components/AboutUsContentTwo.vue';
import AboutUsContentThreeVue from './components/AboutUsContentThree.vue';

import ScanneriOSVue from './components/ScanneriOS.vue';
import ScannerAndroidVue from './components/ScannerAndroid.vue';
import ScannerGoogleVue from './components/ScannerGoogle.vue';

export default {
  name: 'App',
  components: {
    ComponentOne,
    TopMenuButton,
    GreenBox2Vue,
    GreenBox3Vue,
    GreenBox4Vue,
    BenefitsInfo,
    AboutUsContentVue,
    AboutUsContentTwoVue,
    AboutUsContentThreeVue,
    ScanneriOSVue,
    ScannerAndroidVue,
    ScannerGoogleVue

  },
  data() {
    return {
    }
  },
  computed: {
    background() {
      return {
        backgroundImage: `url(${require('@/assets/Backy1.png')})`,
        backgroundSize: 'cover',
        //position: 'relative'
        height: 'auto',
        width: 'auto'
      };
    },
  },
  methods: {
    handleClick() {
      this.$refs.Overview.scrollIntoView({ behavior: 'smooth' });
    },
    handleClick2() {
      this.$refs.Service.scrollIntoView({ behavior: 'smooth' });
    },
    handleClick3() {
      this.$refs.Benefits.scrollIntoView({ behavior: 'smooth' });
    },
    handleClick4() {
      this.$refs.AboutUs.scrollIntoView({ behavior: 'smooth' });
    },
    handleClick5() {
      this.$refs.Contact.scrollIntoView({ behavior: 'smooth' });
    }
  },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.flex {
  display: flex;
  justify-content: start;
  flex-wrap: wrap;
  position: fixed;
  top: 0vh;
  /* left: -5vw; */
  height: 10vh;
  width: 100vw;
  /* margin-right: 100px;
  margin-left: 100px; */
  margin-top: 0px;
  /* background-color:white ; */
  background-image: linear-gradient(white, rgba(255, 255, 255, 0.815), rgba(255, 255, 255, 0.644), rgba(255, 255, 255, 0.514), rgba(255, 255, 255, 0.199), rgba(255, 255, 255, 0));
  opacity: 1;
  z-index: 10000;
  /* border-bottom: .05vh solid;
  border-color: rgba(255, 255, 255, 0.479);
  border-width: thin; */

}

.flex2 {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  margin-right: 100px;
  margin-left: 100px;
  margin-top: 0px;
}

.flex3 {
  display: flex;
  justify-content: space-between;
  flex-wrap: nowrap;
  margin-right: 100px;
  position: fixed;
  left: 32%;
  margin-top: 2vh;
  height: fit-content;
  z-index: 10000;
}

.title2 {
  color: white;
  font-family: var(--font-family-erasitc-bold);
  font-size: var(--font-size-xxx1);
  font-weight: 1000;
  font-style: italic 20deg;
  letter-spacing: 0;
  line-height: 30vh;
  /* min-height: 117px; */
  text-shadow: 7px 7px 1px #277938;
  white-space: nowrap;
  font-size: 10vh;
  /* margin-bottom: 50px; */
  resize: both;
}

.title3 {
  color: #003114;
  font-size: var(--font-size-xxx1);
  font: normal normal 900 4vh Segoe UI;
  height: fit-content;
  flex-wrap: wrap;
  resize: both;
  text-align: left;
  white-space: wrap;

}
</style>
