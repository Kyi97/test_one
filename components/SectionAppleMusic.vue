<template>
  <div class="section-apple-music">
    <div class="section-student-plan">
      <div class="row">
        <div class="copy-container">
          <p class="typography-router-headline">
            The&nbsp;Apple&nbsp;Music Student <br class="small" />Plan comes
            with <br class="small" />Apple&nbsp;TV+ for&nbsp;free.<sup
              class="footnote footnote-number"
              ><a href="#footnote-5" aria-label="Footnote 4">4</a></sup
            >
          </p>
          <a href="#" class="button">Try Apple Music free</a>
        </div>
        <div class="image-wrapper column">
          <div class="image-student-plan"></div>
        </div>
      </div>
    </div>
  </div>
</template>
  <script>
export default {
  name: "SectionAppleMusic",
};
</script>
  <style lang="scss" scoped>
.section-apple-music {
  height: auto;
  position: relative;
  overflow: hidden;
  padding-top: 39px;
  flex-direction: row;
  flex-wrap: wrap;
  resize: vertical;
  margin-left: auto;
  margin-right: auto;
  justify-content: center;
  width: 97%;
  .section-student-plan {
    left: 0;
    height: 530px;
    margin: 0 auto;
    max-width: 1360px;
    position: relative;
    top: 0;
    width: 100%;
    background-color: #f5f5f7;

    .row {
      display: flex;
      flex-wrap: nowrap;
      height: 100%;
      justify-content: space-evenly;
      box-sizing: border-box;
      padding-top: 108px;

      .copy-container-plan {
        height: 100%;
        max-width: 535px;
        margin-right: 20px;
      }
      .typography-router-headline {
        align-items: center;
        margin-left: 3%;
        font-size: 48px;
        line-height: 1.0834933333;
        font-weight: 700;
        letter-spacing: -0.003em;
        font-family: SF Pro Display, SF Pro Icons, Helvetica Neue, Helvetica,
          Arial, sans-serif;

        a {
          text-decoration: none;
        }
      }
      .button {
        margin-top: 13px;
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
        text-decoration: none;
      }
      .image-wrapper {
        display: flex;
        justify-content: center;
        align-items: flex-end;
      }
      .column {
        box-sizing: border-box;
        margin: 0;
        padding: 0;
        min-width: 0px;
      }
      .image-student-plan {
        width: 533px;
        height: 450px;
        background-size: 533px 450px;
        background-repeat: no-repeat;
        background-image: url(https://www.apple.com/v/apple-tv-plus/ag/images/overview/student_plan__bm7yp0v4tf6u_large.jpg);
      }
    }
  }
}
</style>