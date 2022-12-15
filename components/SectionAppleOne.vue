<template>
  <div class="section-apple-one">
    <div class="figure-wrapper large6">
      <div class="tile-image"></div>
    </div>
    <div class="text-container large6">
      <div class="text-wrapper">
        <h2 class="tile-logo">
          <span class="visuallyhidden">Apple One</span>
        </h2>
        <p class="tile-headline typography-router-headline">
          <span>Bundle Apple&nbsp;TV+</span>
          <br />with up to five<br />
          other great&nbsp;services.<br />And enjoy more for less.
        </p>
        <a href="#" class="icon-wrapper button"
          ><span class="icon-copy"
            >Try Apple&nbsp;One free<sup class="footnote footnote-number"
              >3</sup
            ></span
          ></a
        ><br />
        <a href="#" class="icon-wrapper typography-router-cta"
          ><span class="icon-copy">Learn more</span
          ><span class="icon icon-after more"></span
        ></a>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "SectionAppleOne",
};
</script>
<style lang="scss" scoped>
$bgcolor: #f5f5f7;
$display: flex;
.section-apple-one {
  height: auto;
  display: $display;
  background-color: $bgcolor;
  flex-direction: row;
  flex-wrap: wrap;
  resize: vertical;
  margin-left: auto;
  margin-right: auto;
  justify-content: center;
  width: 97%;

  .large-6 {
    flex-basis: 45%;
    max-width: 45%;
  }
  .figure-wrapper {
    justify-content: flex-start;
    position: relative;
    display: $display;

    .tile-image {
      max-width: 544px;
      height: 330px;
      background-image: url(https://www.apple.com/v/apple-tv-plus/ag/images/overview/bundle__e93qdcv7mtm6_large.jpg);
      margin-top: 126px;
      margin-bottom: 128px;
      min-width: 544px;
      margin-left: 3%;
    }
    @media only screen and (max-width: 427px) {
      .tile-image {
        display: none;
      }
    }
  }

  .text-container {
    position: relative;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-start;
    padding-right: 0%;
    box-sizing: border-box;
    .text-wrapper {
      display: $display;
      flex-direction: column;
      align-items: center;
      width: auto;
    }

    .visuallyhidden {
      position: absolute;
      clip: rect(1px, 1px, 1px, 1px);
      -webkit-clip-path: inset(0px 0px 99.9% 99.9%);
      clip-path: inset(0px 0px 99.9% 99.9%);
      overflow: hidden;
      height: 1px;
      width: 1px;
      padding: 0;
      border: 0;
    }
    .tile-headline {
      text-align: center;
      margin-top: 27px;
      margin-bottom: 13px;
    }
    .typography-router-headline {
      font-size: 40px;
      line-height: 1.1;
      font-weight: 700;
      letter-spacing: 0em;
      font-family: SF Pro Display, SF Pro Icons, Helvetica Neue, Helvetica,
        Arial, sans-serif;
    }
    .button {
      display: inline-block;
      text-align: center;
      white-space: nowrap;
      min-width: 28px;
      border-radius: 980px;
      background: #0071e3;
      font-size: 17px;
      line-height: 1.1764805882;
      letter-spacing: -0.022em;
      min-width: 26px;
      padding: 12px 22px;
      font-size: 14px;
      line-height: 1.4285914286;
      font-weight: 400;
      letter-spacing: -0.016em;
      font-family: SF Pro Text, SF Pro Icons, Helvetica Neue, Helvetica, Arial,
        sans-serif;
      font-weight: 700;
      background-color: #fff;
      color: #1d1d1f;
      cursor: pointer;
      color: #fff;
      background-color: #1d1d1f;
    }
    a.icon-wrapper {
      text-decoration: none;
    }
    .typography-router-cta {
      font-size: 19px;
      line-height: 1.2105263158;
      font-weight: 400;
      letter-spacing: 0.012em;
      font-family: SF Pro Display, SF Pro Icons, Helvetica Neue, Helvetica,
        Arial, sans-serif;
    }
  }
}
</style>