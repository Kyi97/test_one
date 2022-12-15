<template>
  <div class="con">
    <div class="container">
      <img
        src="https://www.apple.com/v/apple-tv-plus/ag/images/overview/apple_tv_app_icon__cth1s5qlqpyu_large.png"
      />

      <span class="headline"
        >Watch Apple TB + anywhere on the Apple TV app.</span
      >

      <span class="typography"
        >Find the Apple TV app on your favorite Apple devices. Or watch Apple
        TV+ online at <span class="tv_apple_com">tv.apple.com.</span></span
      >
    </div>

    <div class="build-in">
      <div class="icon-wrapper">
        <img
          class="image-icon-apple-tv"
          src="https://www.apple.com/v/apple-tv-plus/ag/images/overview/icon_apple_tv__r2nel0gcigam_large_2x.jpg"
        />
        <h3 class="feature-headline typography-device-names">Apple&nbsp;TV</h3>
      </div>

      <div class="icon-wrapper">
        <img
          class="image-icon-iphone"
          src="https://www.apple.com/v/apple-tv-plus/ag/images/overview/icon_iphone__c914mkstye0y_large_2x.jpg"
        />
        <h3 class="feature-headline typography-device-names">iPhone</h3>
      </div>

      <div class="icon-wrapper">
        <img
          class="image-icon-ipad"
          src="https://www.apple.com/v/apple-tv-plus/ag/images/overview/icon_ipad__cyk6qow5fiqa_large_2x.jpg"
        />
        <h3 class="feature-headline typography-device-names">iPad</h3>
      </div>

      <div class="icon-wrapper">
        <img
          class="image-icon-mac"
          src="https://www.apple.com/v/apple-tv-plus/ag/images/overview/icon_mac__b7y797p7oouq_large_2x.jpg"
        />
        <h3 class="feature-headline typography-device-names">Mac</h3>
      </div>

      <div class="icon-wrapper">
        <img
          class="image-icon-airplay"
          src="https://www.apple.com/v/apple-tv-plus/ag/images/overview/icon_airplay__ddkvcm0sxtm6_large_2x.jpg"
        />
        <h3 class="feature-headline typography-device-names">AirPlay</h3>
      </div>
    </div>

    <div class="devices-container">
      <div class="see_it">
        See it on your smart TV <br />or streaming device.
      </div>

      <div class="set_up">Set up your device ></div>

      <div class="explore">Explore compatible devices ></div>
    </div>

    <div class="company_container">
      <div>
        <img
          class="image-icon-samsung"
          src="https://www.apple.com/v/apple-tv-plus/ag/images/overview/icon_samsung__er6s8sp9t126_large.jpg"
        />
      </div>
      <div>
        <img
          class="image-icon-lg"
          src="https://www.apple.com/v/apple-tv-plus/ag/images/overview/icon_lg__7fxn3l0zf5ua_large.jpg"
        />
      </div>
      <div>
        <img
          class="image-icon-vizio"
          src="https://www.apple.com/v/apple-tv-plus/ag/images/overview/icon_vizio__crgnno5ezt2e_large.jpg"
        />
      </div>
      <div>
        <img
          class="image-icon-sony"
          src="https://www.apple.com/v/apple-tv-plus/ag/images/overview/icon_sony__dv28xq4n91ea_large.jpg"
        />
      </div>
      <div>
        <img
          class="image-icon-xfinity"
          src="https://www.apple.com/v/apple-tv-plus/ag/images/overview/icon_xfinity__fohor3dbqrmi_large.jpg"
        />
      </div>
      <div>
        <img
          class="image-icon-roku"
          src="https://www.apple.com/v/apple-tv-plus/ag/images/overview/icon_roku__d3kr4gpcimoi_large.jpg"
        />
      </div>
      <div>
        <img
          class="image-icon-firetv"
          src="https://www.apple.com/v/apple-tv-plus/ag/images/overview/icon_firetv__f6qpefrj0ree_large.jpg"
        />
      </div>
      <div>
        <img
          class="image-icon-google-tv"
          src="https://www.apple.com/v/apple-tv-plus/ag/images/overview/icon_google_tv__e5t4asdc2gsy_large.jpg"
        />
      </div>
      <div>
        <img
          class="image-icon-playstation"
          src="https://www.apple.com/v/apple-tv-plus/ag/images/overview/icon_playstation__djtq2b40wf2a_large.jpg"
        />
      </div>
      <div>
        <img
          class="image-icon-xbox"
          src="https://www.apple.com/v/apple-tv-plus/ag/images/overview/icon_xbox__cfelmbxxfoaa_large.jpg"
        />
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "AppleTvApp",
};
</script>

  
  <style lang="scss" scoped>
.con {
  margin-left: auto;
  margin-right: auto;
}

.build-in {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  max-width: 980px;
  resize: vertical;
  gap: 5px;
  height: auto;
  margin-left: auto;
  margin-right: auto;
  justify-content: space-between;
  margin-bottom: 67px;
}

.icon-wrapper {
  display: flex;
  flex-direction: column;
  align-items: center;
}
.image-icon-apple-tv {
  width: 66px;
  height: 82px;
}
.image-icon-iphone {
  width: 90px;
  height: 81px;
}

.image-icon-ipad {
  width: 85px;
  height: 81px;
}

.image-icon-mac {
  width: 114px;
  height: 81px;
}
.image-icon-airplay {
  width: 54px;
  height: 81px;
}

.devices-container {
  display: flex;
  flex-direction: column;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
  text-align: center;
  max-width: 980px;
  margin-left: auto;
  margin-right: auto;

  .see_it {
    font-size: 40px;
    font-weight: bold;
  }
  .set_up,
  .explore {
    color: #0066cc;
    font-size: 17px;
    padding: 5px;
  }
}

.container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  padding-top: 130px;
  max-width: 1100px;
  margin-left: auto;
  margin-right: auto;

  .headline {
    font-size: 4.2vw;
    font-weight: bold;
    margin-top: 10px;
  }
  .typography {
    font-size: 17px;
    margin: 40px 20rem;
    .tv_apple_com {
      color: #0066cc;
    }
  }

  .see_it {
    font-size: 40px;
    font-weight: bold;
    // margin: 0rem 15rem 1rem 15rem;
  }
  .set_up,
  .explore {
    color: #0066cc;
    font-size: 17px;
    padding: 5px;
  }
}
.company_container {
  margin-top: 3rem;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  max-width: 980px;
  resize: vertical;
  gap: 5px;
  margin-left: auto;
  margin-right: auto;
  justify-content: space-between;
}
.company_container > div {
  display: grid;
  place-items: center;
  padding: 0 30px;
}

.build-in > div {
  display: grid;
  place-items: center;
  padding: 0 30px;
}

.image-icon-samsung {
  width: 117px;
  height: 81px;
}
.image-icon-lg {
  width: 161px;
  height: 81px;
}
.image-icon-vizio {
  width: 110px;
  height: 81px;
}
.image-icon-sony {
  width: 126px;
  height: 81px;
}
.image-icon-xfinity {
  width: 113px;
  height: 81px;
}
.image-icon-roku {
  width: 102px;
  height: 81px;
}
.image-icon-firetv {
  width: 96px;
  height: 81px;
}

.image-icon-google-tv {
  width: 160px;
  height: 81px;
}

.image-icon-playstation {
  width: 161px;
  height: 81px;
}
.image-icon-xbox {
  width: 123px;
  height: 81px;
}
img {
  object-fit: contain;
}
</style>