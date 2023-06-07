<template>
  <header class="start" v-show="desktop">
    <div>
      <img src="@/assets/Backy1.png"
        style="height:650vh;width: 100%; position: absolute; top: 0vh; left: 0vw;resize: both;z-index: 0;" />
      <div class="main body" style="height:640vh; background-repeat: no-repeat;">
        <div id="border" style="border:thick">
          <!-- <component-one children="For Shipper" style="background-color: aqua;"/> -->
          <div class="flex">
            <img src="@/assets/logo.png"
              style="height:fit-content; margin-top: 0; position: fixed; top:1vh ;left: 5vw;" />
            <div class="flex3">
              <top-menu-button children="Overview" ref="tester" @click="handleClick" style="width:5;cursor: pointer;" />
              <top-menu-button children="Services" @click="handleClick2" style="width:5;cursor: pointer;" />
              <top-menu-button children="Benefits" @click="handleClick3" style="width:fit-content;cursor: pointer;" />
              <top-menu-button children="About Us" @click="handleClick4" style="width:fit-content;cursor: pointer;" />
              <top-menu-button children="Contact Us" @click="handleClick5" style="width:fit-content;cursor: pointer;" />

            </div>

          </div>
          <div class="Overview" style="position: absolute;top: 10vh; left: 9vw;" ref="Overview">
            <div class="main page" style="height: auto;width: auto;resize: both;">
              <h1 class="title2" style="margin-top: 1vh;">The Route Enterprise</h1>
              <h1 class="title3" style="text-align: center;font-size: 5vh;">Join Us!</h1>
              <h1 class="title3" style="text-align: center;font-size: 5vh;">Scan the QR code and download our App!</h1>
              <div class="flex2">
                <h1 class="title3" style="font-size: 5vh;">We provide</h1>
                <component-one children="integrated," style="background-color: #073E17AD;" />
                <component-one children="efficient," style="background-color: #073E17AD;" />
                <h1 class="title3" style="font-size: 5vh;">and</h1>
                <component-one children="cooperative" style="background-color: #073E17AD;" />
                <h1 class="title3" style="font-size: 5vh;">experience.</h1>
              </div>
            </div>



          </div>

        </div>
        <div class="ServicePage" style="position: absolute;top: 140vh;left: 5vw;" ref="Service">
          <h1
            style="position: absolute; top: 3vh; left: 2vw; font: italic normal bold 5vh Segoe UI;color: white;opacity: 1;">
            Services</h1>

          <green-box2-vue children="For Shipper"
            style="position: absolute; top: 25vh; left: 10vw;background-color: #e3f3e7;height: min-content;" />
          <green-box3-vue children="For Carrier" style="position: absolute; top: 55vh; left: 17vw;height: min-content;" />
          <green-box4-vue children="Tracking Device"
            style="position: absolute; top: 85vh; left: 24vw;height: min-content;" />

          <img src="@/assets/Screen1.png" style="height:65vh; position: absolute; top: 15vh; left: 55vw;resize: both;" />
          <img src="@/assets/Screen2.png" style="height:65vh; position: absolute; top: 45vh; left: 67vw;resize:both" />
          <img src="@/assets/running2.gif" style="height:20vh; position: absolute; top: 67vh; left: 61vw;resize: both;" />
        </div>
        <div class="Benefits Page" style="position: absolute;top: 11vh;">
          <h1 style="position:absolute;top:295vh" ref="Benefits"></h1>
          <h1
            style="position: absolute; top: 300vh; left: 5vw;width: max-content; font: italic normal bold 5vh Segoe UI;color: white;opacity: 1;">
            TRE Partner Benefits</h1>
          <h1 class="title3" style="position: absolute; top: 310vh;left: 5vw; width:48vw;">If you have ambitions, or want
            to get passive income? JOIN US AND BECOME OUR PARTNER! Download App check the benefits details!</h1>
          <img src="@/assets/infographic.png"
            style="height:60vh; position: absolute; top: 310vh; left: 40vw;resize: both;overflow: clip;" />
          <h1
            style="text-align: left;font: normal normal normal 2.6vh Segoe UI;color: #073E17AD;position: absolute;top: 324.5vh;left: 65vw;width: 20vw; resize: both;">
            Downline 1: $？commission/ea. </h1>
          <h1
            style="text-align: left;font: normal normal normal 2.6vh Segoe UI;color: #073E17AD;position: absolute;top: 337vh;left: 65vw;width: 20vw; resize: both;">
            Downline 2: $？commission/ea. </h1>
          <h1
            style="text-align: left;font: normal normal normal 2.6vh Segoe UI;color: #073E17AD;position: absolute;top: 349vh;left: 65vw;width: 20vw; resize: both;">
            Downline 3: $？commission/ea. </h1>
          <h1
            style="text-align: left;font: normal normal normal 2.6vh Segoe UI;color: #073E17AD;position: absolute;top: 362vh;left: 65vw;width: 20vw; resize: both;">
            Downline 4: You receive shares </h1>
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
          <scanner-google-vue style="position: absolute;left: 23vw;top: 15vh;"></scanner-google-vue>
        </div>
        <div class="Contact Page" style="position: absolute; top: 600vh; left: 5vw;">
          <h1 style=" font: italic normal bold 5vh Segoe UI;color: white;opacity: 1;" ref="Contact">Contact Us</h1>
          <img src="@/assets/MapPin.png" style="height:3.5vh; position: absolute; top: 12vh; left: 0vw;" />
          <h1
            style="color:white;position: absolute;top: 11vh;left: 2vw;font: normal normal normal 2vh Segoe UI;width: max-content;">
            3230 Fallow Field Drive Diamond Bar, CA 91765</h1>
          <img src="@/assets/Phone.png" style="height:2.7vh; position: absolute; top: 17vh; left: 0vw;" />
          <h1
            style="color:white;position: absolute;top: 15.5vh;left: 2vw;font: normal normal normal 2vh Segoe UI;width: max-content;">
            909-598-2185</h1>
          <img src="@/assets/Mail.png" style="height:1.9vh; position: absolute; top: 22vh; left: 0vw;" />
          <h1
            style="color:white;position: absolute;top: 20vh;left: 2vw;font: normal normal normal 2vh Segoe UI;width: max-content;">
            info@routeenterprise.com</h1>
          <img src="@/assets/Terms.png" style="height:3vh; position: absolute; top: 27vh; left: 0vw;" />
          <h1
            style="color:white;position: absolute;top: 25.5vh;left: 2vw;font: normal normal normal 2vh Segoe UI;width: max-content;">
            Terms and Conditions</h1>
          <img src="@/assets/Lock.png" style="height:3.1vh; position: absolute; top: 32vh; left: 0vw;" />
          <h1
            style="color:white;position: absolute;top: 31vh;left: 2vw;font: normal normal normal 2vh Segoe UI;width: max-content;">
            Privacy Policy</h1>
          <img src="@/assets/running3.gif"
            style="height:90vh;width: 47vw; position: absolute; top: -45vh; left: 47vw;resize: both;overflow: clip;" />

        </div>

      </div>
    </div>

  </header>





  <!-- <h1 v-show="mobile">aspect ratio too small</h1> -->
  <header v-show="windowed" class="windowed view">
    <div>
      <img src="@/assets/Backy1.png"
        style="height:650vh;width: 100%; position: absolute; top: 0vh; left: 0vw;resize: both;z-index: 0;" />
      <div class="main body" style="height:640vh; background-repeat: no-repeat;">
        <div id="border" style="border:thick">
          <!-- <component-one children="For Shipper" style="background-color: aqua;"/> -->
          <div class="flex">
            <!-- <img src="@/assets/logo.png" style="height:fit-content; margin-top: 0; position: fixed; top:1vh ;left: 5vw;" /> -->
            <div class="flex2">
              <top-menu-button children="Overview" ref="tester" @click="handleClick6" style="width:5;cursor: pointer;" />
              <top-menu-button children="Services" @click="handleClick7" style="width:5;cursor: pointer;" />
              <top-menu-button children="Benefits" @click="handleClick8" style="width:fit-content;cursor: pointer;" />
              <top-menu-button children="About Us" @click="handleClick9" style="width:fit-content;cursor: pointer;" />
              <top-menu-button children="Contact Us" @click="handleClick10" style="width:fit-content;cursor: pointer;" />

            </div>

          </div>
          <div class="Overview" style="position: absolute;top: 10vh; left: 9vw;" ref="Overview1">
            <!-- <div class="main page" style="height: auto;width: auto;resize: both;">
              <h1 class="title2" style="margin-top: 1vh;">The Route Enterprise</h1>
              <h1 class="title3" style="text-align: center;font-size: 5vh;">Join Us!</h1>
              <h1 class="title3" style="text-align: center;font-size: 5vh;">Scan the QR code and download our App!</h1>
              <div class="flex2">
                <h1 class="title3" style="font-size: 5vh;">We provide</h1>
                <component-one children="integrated," style="background-color: #073E17AD;" />
                <component-one children="efficient," style="background-color: #073E17AD;" />
                <h1 class="title3" style="font-size: 5vh;">and</h1>
                <component-one children="cooperative" style="background-color: #073E17AD;" />
                <h1 class="title3" style="font-size: 5vh;">experience.</h1>
              </div>
            </div> -->



          </div>

        </div>
        <div class="ServicePage" style="position: absolute;top: 140vh;left: 5vw;" ref="Service1">
          <h1
            style="position: absolute; top: 3vh; left: 2vw; font: italic normal bold 5vh Segoe UI;color: white;opacity: 1;">
            Services</h1>

          <green-box2-vue children="For Shipper"
            style="position: absolute; top: 25vh; left: 10vw;background-color: #e3f3e7;height: min-content;width: 50vw;" />
          <green-box3-vue children="For Carrier"
            style="position: absolute; top: 55vh; left: 10vw;height: min-content;width: 50vw;" />
          <green-box4-vue children="Tracking Device"
            style="position: absolute; top: 85vh; left: 10vw;height: min-content;width: 50vw;" />

          <!-- <img src="@/assets/Screen1.png" style="height:65vh; position: absolute; top: 15vh; left: 55vw;resize: both;" />
          <img src="@/assets/Screen2.png" style="height:65vh; position: absolute; top: 45vh; left: 67vw;resize:both" />
          <img src="@/assets/running2.gif" style="height:20vh; position: absolute; top: 67vh; left: 61vw;resize: both;" /> -->
        </div>
        <div class="Benefits Page" style="position: absolute;top: 11vh;">
          <h1 style="position:absolute;top:295vh" ref="Benefits1"></h1>
          <h1
            style="position: absolute; top: 300vh; left: 5vw;width: max-content; font: italic normal bold 5vh Segoe UI;color: white;opacity: 1;">
            TRE Partner Benefits</h1>
          <h1 class="title3" style="position: absolute; top: 310vh;left: 5vw; width:48vw;">If you have ambitions, or want
            to get passive income? JOIN US AND BECOME OUR PARTNER! Download App check the benefits details!</h1>
          <!-- <img src="@/assets/infographic.png" style="height:60vh; position: absolute; top: 310vh; left: 40vw;resize: both;overflow: clip;" />
          <h1 style="text-align: left;font: normal normal normal 2.6vh Segoe UI;color: #073E17AD;position: absolute;top: 324.5vh;left: 65vw;width: 20vw; resize: both;">Downline 1: $？commission/ea. </h1>
          <h1 style="text-align: left;font: normal normal normal 2.6vh Segoe UI;color: #073E17AD;position: absolute;top: 337vh;left: 65vw;width: 20vw; resize: both;">Downline 2: $？commission/ea. </h1>
          <h1 style="text-align: left;font: normal normal normal 2.6vh Segoe UI;color: #073E17AD;position: absolute;top: 349vh;left: 65vw;width: 20vw; resize: both;">Downline 3: $？commission/ea. </h1>
          <h1 style="text-align: left;font: normal normal normal 2.6vh Segoe UI;color: #073E17AD;position: absolute;top: 362vh;left: 65vw;width: 20vw; resize: both;">Downline 4: You receive shares </h1> -->
          <benefits-info style="position: absolute;top: 360vh;  width: 75vw;"></benefits-info>
        </div>
        <h1 style="position:absolute;top:415vh" ref="AboutUs1"></h1>
        <div class="About us Page" style="position: absolute; top: 420vh; left: 5vw;">

          <h1 style=" font: italic normal bold 5vh Segoe UI;color: white;opacity: 1;">About Us</h1>
          <about-us-content-vue
            style="position: absolute; top: 15vh;left:5vw;width: 70vw;height: min-content;"></about-us-content-vue>
          <about-us-content-two-vue
            style="position: absolute; top: 50vh;left:5vw;width: 70vw;height: min-content;"></about-us-content-two-vue>
          <about-us-content-three-vue
            style="position: absolute; top: 82vh;left:5vw;width: 70vw;height: min-content;"></about-us-content-three-vue>
        </div>
        <div class="Join Us" style="position: absolute; top: 530vh; left: 5vw;">
          <h1 style=" font: italic normal bold 5vh Segoe UI;color: white;opacity: 1;" ref="Join1">Join Us</h1>
          <scanneri-o-s-vue style="position: absolute;left: 0vw;top: 15vh;resize: both; "></scanneri-o-s-vue>
          <scanner-google-vue style="position: absolute;left: 23vw;top: 15vh;"></scanner-google-vue>
        </div>
        <div class="Contact Page" style="position: absolute; top: 600vh; left: 5vw;">
          <h1 style=" font: italic normal bold 5vh Segoe UI;color: white;opacity: 1;" ref="Contact1">Contact Us</h1>
          <img src="@/assets/MapPin.png" style="height:3.5vh; position: absolute; top: 12vh; left: 0vw;" />
          <h1
            style="color:white;position: absolute;top: 11vh;left: 5vw;font: normal normal normal 2vh Segoe UI;width: max-content;">
            3230 Fallow Field Drive Diamond Bar, CA 91765</h1>
          <img src="@/assets/Phone.png" style="height:2.7vh; position: absolute; top: 17vh; left: 0vw;" />
          <h1
            style="color:white;position: absolute;top: 15.5vh;left: 5vw;font: normal normal normal 2vh Segoe UI;width: max-content;">
            909-598-2185</h1>
          <img src="@/assets/Mail.png" style="height:1.9vh; position: absolute; top: 22vh; left: 0vw;" />
          <h1
            style="color:white;position: absolute;top: 20vh;left: 5vw;font: normal normal normal 2vh Segoe UI;width: max-content;">
            info@routeenterprise.com</h1>
          <img src="@/assets/Terms.png" style="height:3vh; position: absolute; top: 27vh; left: 0vw;" />
          <h1
            style="color:white;position: absolute;top: 25.5vh;left: 5vw;font: normal normal normal 2vh Segoe UI;width: max-content;">
            Terms and Conditions</h1>
          <img src="@/assets/Lock.png" style="height:3.1vh; position: absolute; top: 32vh; left: 0vw;" />
          <h1
            style="color:white;position: absolute;top: 31vh;left: 5vw;font: normal normal normal 2vh Segoe UI;width: max-content;">
            Privacy Policy</h1>
          <img src="@/assets/running3.gif"
            style="height:90vh;width: 47vw; position: absolute; top: -45vh; left: 47vw;resize: both;overflow: clip;" />

        </div>

      </div>
    </div>
  </header>






  <header v-show="mobile" class="mobile view">
    <div>
      
      <TheSidebar :open="navOpen"/>
      <img src="@/assets/MobileBacky2.png"
        style="height:650vh;width: 100%; position: absolute; top: 0vh; left: 0vw;resize: both;z-index: 0;" />
      <div class="main body" style="height:640vh; background-repeat: no-repeat;">
        <div id="border" style="border:thick">
          <!-- <component-one children="For Shipper" style="background-color: aqua;"/> -->
          <div class="flex" style="justify-content: center;">
            <img src="@/assets/logo.png"
              style="height:fit-content; margin-top: 0; position: fixed; top:1vh ;left: 5vw;" />
            <!-- <div class="flex2">
              <top-menu-button children="Overview" ref="tester" @click="handleClick11" style="width:5;cursor: pointer;" />
              <top-menu-button children="Services" @click="handleClick12" style="width:5;cursor: pointer;" />
              <top-menu-button children="Benefits" @click="handleClick13" style="width:fit-content;cursor: pointer;" />
              <top-menu-button children="About Us" @click="handleClick14" style="width:fit-content;cursor: pointer;" />
              <top-menu-button children="Contact Us" @click="handleClick15" style="width:fit-content;cursor: pointer;" />

            </div> -->

          </div>
          <div class="Overview" style="position: absolute;top: 10vh; left: 0vw;" ref="Overview2">
            <div class="main page" style="height: auto;width: auto;resize: both;">
              <h1 class="title2" style="margin-top: 1vh;font-size:8vw; width:100vw">The Route Enterprise</h1>
              <h1 class="title3" style="text-align: center;font-size: 8vw;width:100vw">Join Us!</h1>
              <h1 class="title3" style="text-align: center;font-size: 7vw;width:100vw">Scan the QR code and download our App!</h1>
              <div class="flex2" style="width:100vw;position:absolute;top:55vh;left:-25vw">
                <h1 class="title3" style="font-size: 7vw;">We provide</h1>
                <component-one-mobile-vue children="integrated," style="background-color: #073E17AD;" />
                <component-one-mobile-vue children="efficient," style="background-color: #073E17AD;" />
                <h1 class="title3" style="font-size: 7vw;">and</h1>
                <component-one-mobile-vue children="cooperative" style="background-color: #073E17AD;" />
                <h1 class="title3" style="font-size: 7vw;">experience.</h1>
              </div>
            </div>



          </div>

        </div>
        <div class="ServicePage" style="position: absolute;top: 140vh;left: 5vw;" ref="Service2">
          <h1
            style="position: absolute; top: 3vh; left: 2vw; font: italic normal bold 5vh Segoe UI;color: white;opacity: 1;">
            Services</h1>

          <mobile-green-box2 children="For Shipper"
            style="position: absolute; top: 25vh; left: 3vw;background-color: #e3f3e7;" />
          <mobile-green-box3-vue children="For Carrier" style="position: absolute; top: 55vh; left: 3vw;" />
          <mobile-green-box4-vue children="Tracking Device" style="position: absolute; top: 85vh; left: 3vw;" />

          <!-- <img src="@/assets/Screen1.png" style="height:65vh; position: absolute; top: 15vh; left: 55vw;resize: both;" />
          <img src="@/assets/Screen2.png" style="height:65vh; position: absolute; top: 45vh; left: 67vw;resize:both" />
          <img src="@/assets/running2.gif" style="height:20vh; position: absolute; top: 67vh; left: 61vw;resize: both;" /> -->
        </div>
        <div class="Benefits Page" style="position: absolute;top: 11vh;">
          <h1 style="position:absolute;top:295vh" ref="Benefits2"></h1>
          <h1
            style="position: absolute; top: 300vh; left: 5vw;width: max-content; font: italic normal bold 5vh Segoe UI;color: white;opacity: 1;">
            TRE Partner Benefits</h1>
          <h1 class="title3"
            style="position: absolute; top: 310vh;left: 11vw; width:75vw;font-size: 3vh;text-align: center;">If you have
            ambitions, or want
            to get passive income? JOIN US AND BECOME OUR PARTNER! Download App check the benefits details!</h1>
          <!-- <img src="@/assets/infographic.png" style="height:60vh; position: absolute; top: 310vh; left: 40vw;resize: both;overflow: clip;" />
          <h1 style="text-align: left;font: normal normal normal 2.6vh Segoe UI;color: #073E17AD;position: absolute;top: 324.5vh;left: 65vw;width: 20vw; resize: both;">Downline 1: $？commission/ea. </h1>
          <h1 style="text-align: left;font: normal normal normal 2.6vh Segoe UI;color: #073E17AD;position: absolute;top: 337vh;left: 65vw;width: 20vw; resize: both;">Downline 2: $？commission/ea. </h1>
          <h1 style="text-align: left;font: normal normal normal 2.6vh Segoe UI;color: #073E17AD;position: absolute;top: 349vh;left: 65vw;width: 20vw; resize: both;">Downline 3: $？commission/ea. </h1>
          <h1 style="text-align: left;font: normal normal normal 2.6vh Segoe UI;color: #073E17AD;position: absolute;top: 362vh;left: 65vw;width: 20vw; resize: both;">Downline 4: You receive shares </h1> -->
          
          <div class="benefits-info"  style="position: absolute;top: 340vh;  width: 85vw;left: -2vw;border-radius:20px" >
        <h1 class="benefits-font" style="text-align: center;font-size: 2.5vh;">Encourage new users to join TRE networks, they become your downline, and you can earn commissions generated by those individuals. Your downline also recruits new downlines into the company, create a hierarchy of partnership, with those at the top of the organization earning commissions on the downlines beneath them.</h1>
    </div>
        </div>
        <h1 style="position:absolute;top:415vh" ref="AboutUs2"></h1>
        <div class="About us Page" style="position: absolute; top: 420vh; left: 5vw;">

          <h1 style=" font: italic normal bold 5vh Segoe UI;color: white;opacity: 1;">About Us</h1>
          <div class="about-us" style="justify-content: center;width: 85vw;position: absolute; top: 10vh;left:2vw;height: min-content;">
            <img src="@/assets/ShakingHands.png" style="height:9vh;margin-top: 4vh;" />
            <h1 class="about-us-font">TRE is a company that has a strong spirit of cooperation, hence we provide
              partnership. Helps you earn passive income.</h1>
          </div>
          <div class="about-us" style="justify-content: center;width: 85vw;position: absolute; top: 48vh;left:2vw;height: min-content;">
            <img src="@/assets/Target.png" style="height:9vh;margin-top: 4vh;" />
            <h1 class="about-us-font">TRE has track devices and technology to help you better protect your truck goods.</h1>
          </div>
          <div class="about-us" style="justify-content: center;width: 85vw;position: absolute; top: 83vh;left:2vw;height: min-content;">
            <img src="@/assets/Exchange.png" style="height:9vh;margin-top: 4vh;" />
        <h1 class="about-us-font">TRE is open platform provide carrier & shipper more opportunity & better experience.</h1>
          </div>
          
        </div>
        <div class="Join Us" style="position: absolute; top: 535vh; left: 5vw;">
          <h1 style=" font: italic normal bold 5vh Segoe UI;color: white;opacity: 1;" ref="Join2">Join Us</h1>
          <!-- <scanneri-o-s-vue style="position: absolute;left: 0vw;top: 15vh;resize: both;height: 10vh; "></scanneri-o-s-vue> -->
          <div class="scanner" style="justify-content: center;position: absolute;left: 14vw;top: 15vh;height: 17vh;width: 12vh;">
        <img src="@/assets/RickRoll.png" style="width:20vw;position: absolute;top:1vh;left: 2vw;" />
        <img src="@/assets/Apple.png" style="height:4.5vh;position: absolute;top: 11.5vh;left: 8vw;" />
        <!-- <h1 class="about-us-font">TRE is a company that has a strong spirit of cooperation, hence we provide partnership. Helps you earn passive income.</h1> -->


    </div>
          
    <div class="scanner" style="justify-content: center;position: absolute;left: 50vw;top: 15vh;height: 17vh;width: 12vh;">
        <img src="@/assets/RickRoll.png" style="width:20vw;position: absolute;top:1vh;left: 2vw; resize: both;" />
        <img src="@/assets/GooglePlay.png" style="height:4.5vh;position: absolute;top: 11.5vh;left: 8vw;" />
        <!-- <h1 class="about-us-font">TRE is a company that has a strong spirit of cooperation, hence we provide partnership. Helps you earn passive income.</h1> -->


    </div>
    <img src="@/assets/running3.gif"
            style="height:40vh; position: absolute; top: 29vh; left: 5vw;resize: both;overflow: clip;" />
        </div>
        <div class="Contact Page" style="position: absolute; top: 600vh; left: 5vw;">
          <h1 style=" font: italic normal bold 5vh Segoe UI;color: white;opacity: 1;" ref="Contact2">Contact Us</h1>
          <img src="@/assets/MapPin.png" style="height:3.5vh; position: absolute; top: 12vh; left: 0vw;" />
          <h1
            style="color:white;position: absolute;top: 11.5vh;left: 9vw;font: normal normal normal 1.8vh Segoe UI;width: max-content;">
            3230 Fallow Field Drive Diamond Bar, CA 91765</h1>
          <img src="@/assets/Phone.png" style="height:2.7vh; position: absolute; top: 17vh; left: 0vw;" />
          <h1
            style="color:white;position: absolute;top: 15.5vh;left: 9vw;font: normal normal normal 1.8vh Segoe UI;width: max-content;">
            909-598-2185</h1>
          <img src="@/assets/Mail.png" style="height:1.9vh; position: absolute; top: 22vh; left: 0vw;" />
          <h1
            style="color:white;position: absolute;top: 20vh;left: 9vw;font: normal normal normal 1.8vh Segoe UI;width: max-content;">
            info@routeenterprise.com</h1>
          <img src="@/assets/Terms.png" style="height:3vh; position: absolute; top: 27vh; left: 0vw;" />
          <h1
            style="color:white;position: absolute;top: 25.5vh;left: 9vw;font: normal normal normal 1.8vh Segoe UI;width: max-content;">
            Terms and Conditions</h1>
          <img src="@/assets/Lock.png" style="height:3.1vh; position: absolute; top: 32vh; left: 0vw;" />
          <h1
            style="color:white;position: absolute;top: 31vh;left: 9vw;font: normal normal normal 1.8vh Segoe UI;width: max-content;">
            Privacy Policy</h1>
          

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
import ScannerGoogleVue from './components/ScannerGoogle.vue';
import MobileGreenBox2 from './components/MobileGreenBox2.vue';
import MobileGreenBox3Vue from './components/MobileGreenBox3.vue';
import MobileGreenBox4Vue from './components/MobileGreenBox4.vue';

import TheSidebar from './components/TheSidebar'
import ComponentOneMobileVue from './components/ComponentOneMobile.vue';

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
    ScannerGoogleVue,
    MobileGreenBox2,
    MobileGreenBox3Vue,
    MobileGreenBox4Vue,
    TheSidebar,
    ComponentOneMobileVue



  },
  data() {
    return {
      navOpen: false
    }
  },
  created() {
    window.addEventListener("resize", this.checkScreen);
    this.checkScreen();
  },
  computed: {
    background() {
      return {
        backgroundImage: `url(${require('@/assets/Backy1.png')})`,
        backgroundSize: 'cover',
        //position: 'relative'
        height: 'auto',
        width: 'auto',

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
    },
    handleClick6() {
      this.$refs.Overview1.scrollIntoView({ behavior: 'smooth' });
    },
    handleClick7() {
      this.$refs.Service1.scrollIntoView({ behavior: 'smooth' });
    },
    handleClick8() {
      this.$refs.Benefits1.scrollIntoView({ behavior: 'smooth' });
    },
    handleClick9() {
      this.$refs.AboutUs1.scrollIntoView({ behavior: 'smooth' });
    },
    handleClick10() {
      this.$refs.Contact1.scrollIntoView({ behavior: 'smooth' });
    },
    handleClick11() {
      this.$refs.Overview2.scrollIntoView({ behavior: 'smooth' });
    },
    handleClick12() {
      this.$refs.Service2.scrollIntoView({ behavior: 'smooth' });
    },
    handleClick13() {
      this.$refs.Benefits2.scrollIntoView({ behavior: 'smooth' });
    },
    handleClick14() {
      this.$refs.AboutUs2.scrollIntoView({ behavior: 'smooth' });
    },
    handleClick15() {
      this.$refs.Contact2.scrollIntoView({ behavior: 'smooth' });
    },
    checkScreen() {
      this.windowWidth = window.innerWidth;
      if (this.windowWidth <= 700) {
        this.mobile = true;
        this.windowed = false;
        this.desktop = false;
        return
      }
      else if (this.windowWidth <= 1000) {
        this.windowed = true;
        this.mobile = false;
        this.desktop = false;
        return
      }
      this.windowed = false;
      this.mobile = false;
      this.desktop = true;
    },
    boxWidth() {
      return GreenBox2Vue.width;

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

/* .background{
  transition: 1ms;
  visibility: hidden;
} */
/* .background:hover{
  
} */

.flex {
  display: flex;
  justify-content: start;
  flex-wrap: wrap;
  position: fixed;
  top: 0vh;
  left: 0vw;
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
  left: 30vw;
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
  transition: 1s;
}

.title2:hover {
  transform: scale(1.05);
}

.title3 {
  color: #003114;
  /* font-size: var(--font-size-xxx1); */
  font: normal normal 900 4vh Segoe UI;
  height: fit-content;
  flex-wrap: wrap;
  resize: both;
  text-align: left;
  white-space: wrap;

}</style>
