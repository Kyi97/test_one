<template>
  <div class="container">
    <div class="nav_container">
      <div class="nav">
        <div>
          <img src="https://img.icons8.com/office/17/null/mac-os.png" />
        </div>
        <div>Store</div>
        <div>Mac</div>
        <div>iPad</div>
        <div>iPhone</div>
        <div>Watch</div>
        <div>AirPods</div>
        <div>TV & Home</div>
        <div>Only on Apple</div>
        <div>Accessories</div>
        <div>Support</div>
        <div>
          <img
            src="https://img.icons8.com/fluency-systems-regular/17/FFFFFF/search--v1.png"
          />
        </div>
        <div>
          <img src="https://img.icons8.com/windows/17/FFFFFF/store-front.png" />
        </div>
      </div>
    </div>
    <div class="stream_now_container">
      <div class="apple_tv">Apple TV+</div>
      <div class="stream_now">Stream now</div>
    </div>
    <div class="notify_container">
      <div style="display: flex">
        MLS Season Pass. Stream every Major League Soccer match. Coming soon.*
        <div class="notify_me">&nbsp;Notify me ></div>
      </div>
    </div>
  </div>
</template>
  
  <script>
export default {
  name: "NavBar",
};
</script>
  
  <style lang="scss" scoped>
$nav-color: #000;
$text-color: #f5f5f7;
.container {
  background-color: #1d1d1f;
  font-family: "SF Pro Text", "Myriad Set Pro", "SF Pro Icons", "Helvetica Neue",
    "Helvetica", "Arial", sans-serif;
  @media only screen and (max-width: 720px) {
    .nav_container {
      display: none;
    }
  }
  .nav_container {
    background-color: $nav-color;
    height: 44px;
    width: auto;
    padding: 0 1rem;
    .nav {
      display: flex;
      height: 44px;
      justify-content: space-between;
      align-items: center;
      color: $text-color;
      font-size: 12px;
      font-weight: 400;
      max-width: 980px;
      z-index: 2;
      margin-left: auto;
      margin-right: auto;
    }
  }

  .stream_now_container {
    height: 52px;
    // padding: 0 29rem;
    display: flex;
    justify-content: space-between;
    max-width: 980px;
    align-items: center;
    margin-left: auto;
    margin-right: auto;
    padding: 0 1rem;
    .apple_tv {
      color: #ffffff;
      font-size: 21px;
      font-weight: bold;
    }
    .stream_now {
      display: flex;
      justify-content: space-between;
      align-items: center;
      background-color: #ffffff;
      padding: 5px 8px;
      border-radius: 20px;
      font-size: 12px;
      letter-spacing: 0.5px;
      font-weight: 100;
    }
  }

  .notify_container {
    height: 52px;
    display: flex;
    font-size: 14px;
    justify-content: center;
    align-items: center;
    color: #f5f5f7;
    border-top: 1px solid rgb(255, 255, 255, 0.3);
    padding: 0 1rem;
    .notify_me {
      color: #2997ff;
      cursor: pointer;
    }
  }
}
</style>