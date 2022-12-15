<template>
  <div class="container">
    <div class="tv-4k">
      <figure class="image-apple-tv-4k"></figure>
      <div class="copy-container">
        <span class="violator-frameless">New</span>
        <h3 class="tv-4k-icon"></h3>
        <p class="typography-router-headline">
          The Apple experience.<br />Cinematic in every&nbsp;sense.
        </p>
        <div class="typography-router-cta ctas large-12 large-centered">
          <ul class="links-inline">
            <li>
              <a href="#" class="icon-wrapper button button-elevated"
                ><span class="icon-copy">Buy</span></a
              >
            </li>
            <li>
              <a href="#" class="icon-wrapper learn-more"
                ><span class="icon-copy">Learn more</span
                ><span class="icon icon-after more"></span
              ></a>
            </li>
          </ul>
        </div>
      </div>
    </div>
    <div
      class="airplay-router"
      data-analytics-section-engagement="name:airplay"
    >
      <figure class="image-router-airplay"></figure>
      <div class="copy-container">
        <h3 class="typography-router-eyebrow icon">AirPlay</h3>
        <p class="typography-router-headline headline">
          Bring Apple&nbsp;TV+ to <br />a screen near you.
        </p>
        <a
          href="/airplay/"
          data-analytics-title="learn more about airplay"
          aria-label="learn more about airplay"
          class="icon-wrapper typography-router-cta learn-more"
          ><span class="icon-copy">Learn more</span
          ><span class="icon icon-after more"></span
        ></a>
      </div>
    </div>
  </div>
</template>
  <script lang="ts">
import Vue from "vue";
export default Vue.extend({});
</script>
  <style lang="scss" scoped>
.container {
  position: relative;
  max-width: 1360px;
  margin: 40px auto;
  display: flex;
  justify-content: space-between;
  .tv-4k {
    width: 48.5%;
    height: 100%;
    background-color: #f5f5f7;
    justify-content: center;
    display: flex;
  }
  .airplay-router,
  .tv-4k {
    position: relative;
    transform: translate(0px);
    overflow: hidden;
    min-height: 880px;
    display: flex;
    flex-direction: column;
  }
  figure {
    display: block;
    margin-block-start: 1em;
    margin-block-end: 1em;
    margin-inline-start: 40px;
    margin-inline-end: 40px;
  }

  .image-apple-tv-4k {
    width: 663px;
    height: 494px;
    background-size: 663px 494px;
    background-repeat: no-repeat;
    background-image: url(https://www.apple.com/v/apple-tv-plus/ag/images/overview/apple_tv_4k_remote__igmcbznr1w2u_large.jpg);
    position: relative;
    left: 50%;
    margin-left: -331.5px;
    background-position: bottom;
    bottom: 0;
    z-index: -1;
    order: 1;
    min-height: 567px;
  }
  .copy-container {
    position: relative;
    width: 100%;
    padding-bottom: 100px;
    top: 106px;
  }
  .lcontainer .copy-container .violator-frameless {
    position: absolute;
    width: 100%;
    text-align: center;
    top: -34px;
  }
  .violator-frameless {
    box-sizing: border-box;
    white-space: nowrap;
    display: block;
    color: #bf4800;
  }
  .tv-4k-icon {
    width: 116px;
    height: 35px;
    background-size: 116px 35px;
    background-repeat: no-repeat;
    background-image: url(https://www.apple.com/v/apple-tv-plus/ag/images/overview/apple_tv_4k_logo__bx1mtrage32a_large.png);
    position: relative;
    left: 50%;
    margin-left: -58px;
    margin-bottom: 15px;
  }
  .container .typography-router-headline {
    margin-top: 21px;
    margin-bottom: 17px;
  }
  .typography-router-headline {
    font-size: 48px;
    line-height: 1.0834933333;
    font-weight: 700;
    letter-spacing: -0.003em;
    font-family: SF Pro Display, SF Pro Icons, Helvetica Neue, Helvetica, Arial,
      sans-serif;
  }
  .typography-router-cta {
    font-size: 19px;
    line-height: 1.2105263158;
    font-weight: 400;
    letter-spacing: 0.012em;
    font-family: SF Pro Display, SF Pro Icons, Helvetica Neue, Helvetica, Arial,
      sans-serif;
  }
  .links-inline,
  .links-stacked {
    margin-left: 0;
    margin-right: 0;
    list-style: none;
  }
  .links-inline li:first-child {
    margin-left: 0;
  }
  .links-inline li {
    display: inline;
    margin: 0 0.8em;
  }
  .button {
    color: #fff;
  }

  a.icon-wrapper {
    text-decoration: none;
  }
  .button {
    cursor: pointer;
    display: inline-block;
    text-align: center;
    white-space: nowrap;
    font-size: 17px;
    line-height: 1.1764805882;
    font-weight: 400;
    letter-spacing: -0.022em;
    font-family: SF Pro Text, SF Pro Icons, Helvetica Neue, Helvetica, Arial,
      sans-serif;
    min-width: 28px;
    padding: 8px 16px;
    border-radius: 980px;
    background: #0071e3;
    color: #fff;
  }
}
</style>