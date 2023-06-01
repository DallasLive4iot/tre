<template>
  <header class="start">
    <div v-bind:style="background">
      <div class="main body" style="height:640vh; background-repeat: no-repeat;">
        <div id="border" style="border:thick">
          <!-- <component-one children="For Shipper" style="background-color: aqua;"/> -->
          <div class="flex">
            <img src="@/assets/logo.png" style="height:50px; margin-top: 0; position: absolute; top: 4%;" ref="Overview"/>
            <div class="flex3">
              <top-menu-button children="Overview" @click="handleClick" style="width:5" />
            <top-menu-button children="Services" @click="handleClick2" style="width:fit-content" />
            <top-menu-button children="Benefits" @click="handleClick3" style="width:fit-content" />
            <top-menu-button children="About Us" @click="handleClick4" style="width:fit-content" />
            <top-menu-button children="Contact Us" @click="handleClick5" style="width:fit-content" />

            </div>
            
          </div>
          <div class="main page">
            <h1 class="title2" style="margin-top: 30vh;">The Route Enterprise</h1>
          <h1 class="title3">Join Us!</h1>
          <h1 class="title3">Scan the QR code and download our App!</h1>
          <div class="flex2">
            <h1 class="title3">We provide</h1>
            <component-one children="integrated," style="background-color: #073E17AD;" />
            <component-one children="efficient," style="background-color: #073E17AD;" />
            <h1 class="title3">and</h1>
            <component-one children="integrated," style="background-color: #073E17AD;" />
            <h1 class="title3">experience.</h1>
          </div>
          

          </div>

        </div>
        <div class="ServicePage">
          <h1
            style="position: absolute; top: 160vh; left: 5vw; font: italic normal bold 45px/60px Segoe UI;color: white;opacity: 1;"
            ref="Service">Services</h1>

          <green-box2-vue children="For Shipper" style="position: absolute; top: 175vh; left: 10vw;background-color: #e3f3e7;" />
          <green-box3-vue children="For Carrier" style="position: absolute; top: 205vh; left: 17vw;" />
          <green-box4-vue children="Tracking Device" style="position: absolute; top: 235vh; left: 24vw;" />
          <img src="@/assets/OBD.png" style="height:290px; position: absolute; top: 242vh; left: 40vw;" />
          <img src="@/assets/Screen1.png" style="height:630px; position: absolute; top: 165vh; left: 55vw;" />
          <img src="@/assets/Screen2.png" style="height:630px; position: absolute; top: 195vh; left: 67vw;" />
          <img src="@/assets/running2.gif" style="height:224px; position: absolute; top: 217vh; left: 59vw;" />
        </div>
        <div class="Benefits Page">
          <h1
            style="position: absolute; top: 300vh; left: 5vw; font: italic normal bold 45px/60px Segoe UI;color: white;opacity: 1;"
            ref="Benefits">Benefits</h1>
            <h1 class="title3" style="position: absolute; top: 310vh;left: 5vw; width:45vw;text-align: left;">If you have ambitions, or want to get passive income? JOIN US AND BECOME OUR PARTNER! Download App check the benefits details!</h1> 
        </div>
        <div class="About us Page" style="position: absolute; top: 400vh; left: 5vw;">
          <h1
            style=" font: italic normal bold 45px/60px Segoe UI;color: white;opacity: 1;"
            ref="AboutUs">About Us</h1>
        </div>
        <div class="Join Us" style="position: absolute; top: 500vh; left: 5vw;">
          <h1
            style=" font: italic normal bold 45px/60px Segoe UI;color: white;opacity: 1;"
            ref="Join">Join Us</h1>
        </div>
        <div class="Contact Page" style="position: absolute; top: 600vh; left: 5vw;">
          <h1
            style=" font: italic normal bold 45px/60px Segoe UI;color: white;opacity: 1;"
            ref="Contact">Contact Us</h1>
            <img src="@/assets/MapPin.png" style="height:34px; position: absolute; top: 12vh; left: 0vw;" />
            <img src="@/assets/Phone.png" style="height:27px; position: absolute; top: 17vh; left: 0vw;" />
            <img src="@/assets/Mail.png" style="height:18px; position: absolute; top: 22vh; left: 0vw;" />
            <img src="@/assets/Terms.png" style="height:28px; position: absolute; top: 27vh; left: 0vw;" />
            <img src="@/assets/Lock.png" style="height:30px; position: absolute; top: 32vh; left: 0vw;" />
            <img src="@/assets/running3.gif" style="height:800px; position: absolute; top: -25vh; left: 50vw;" />
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

export default {
  name: 'App',
  components: {
    ComponentOne,
    TopMenuButton,
    GreenBox2Vue,
    GreenBox3Vue,
    GreenBox4Vue,


  },
  data() {
    return {
    }
  },
  computed: {
    background() {
      return {
        backgroundImage: `url(${require('@/assets/Backy1.png')})`,
        backgroundSize: 'cover  '
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
  justify-content: left;
  flex-wrap: wrap;
  margin-right: 100px;
  margin-left: 100px;
  margin-top: 0px;  
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
  flex-wrap: wrap;
  margin-right: 100px;
  position: fixed;
  left: 32%;
  margin-top: 0px;
}
.title2 {
  color: white;
  font-family: var(--font-family-erasitc-bold);
  font-size: var(--font-size-xxx1);
  font-weight: 1000;
  font-style: italic 20deg;
  letter-spacing: 0;
  line-height: 100px;
  min-height: 117px;
  text-shadow: 7px 7px 1px #277938;
  white-space: nowrap;
  font-size: 90px;
  margin-bottom: 50px;
}

.title3 {
  color: #003114;
  font: normal normal 900 36px/49px Segoe UI;
  height: 25px;
  flex-wrap: wrap;
}</style>
