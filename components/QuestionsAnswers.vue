<template>
  <div class="section">
    <h2 class="typography-app-headline">Questions? Answers.</h2>
    <div v-for="(item, i) of items" :key="i" class="list">
      <div>
        <button v-on:click="item.isShow = !item.isShow" class="collapsible">
          <span class="btn">{{ item.Question }}</span>
          <span>
            <img
              v-if="!item.isShow"
              src="https://img.icons8.com/ios-glyphs/30/000000/expand-arrow--v1.png"
            />
            <img
              v-if="item.isShow"
              src="https://img.icons8.com/ios-glyphs/30/000000/collapse-arrow.png"
            />
          </span>
        </button>
      </div>
      <div>
        <transition name="fade">
          <p v-if="item.isShow">
            {{ item.Answer }}
          </p>
        </transition>
      </div>
    </div>
  </div>
</template>
    
    <script>
export default {
  name: "QuestionsAnswers",
  components: {},
  data() {
    return {
      items: [
        {
          Question: "What is Apple TV+?",
          Answer:
            "Apple TV+ is a streaming service featuring Apple Originals — award-winning series, compelling dramas, groundbreaking documentaries, kids’ entertainment, comedies, and more — with new Apple Originals added every month.",
          isShow: false,
        },
        {
          Question: "How can I watch it?",
          Answer:
            "Watch Apple TV+ on the Apple TV app, which is already on your favorite Apple devices. Just open the app, click or tap Apple TV+, and enjoy the shows and movies. You can also watch Apple TV+ on streaming platforms, popular smart TVs, and AirPlay-enabled TVs with the Apple TV app — or watch online at tv.apple.com.",
          isShow: false,
        },
        {
          Question: "What does it cost?",
          Answer:
            "That all depends on which offer you choose. (1) If you buy an Apple device, Apple TV+ is included free for 3 months.1 (2) A monthly subscription is just $6.99 per month after a free seven-day trial.2 (3) Apple TV+ is included in Apple One, which bundles up to five other Apple services into a single monthly subscription. Apple One plans start at $16.95 per month. (4) The Apple Music Student Plan comes with a free subscription to Apple TV+.4",
          isShow: false,
        },
        {
          Question: "Can I share with my family?",
          Answer:
            "Of course. Apple TV+ lets you share your subscription with up to five family members.",
          isShow: false,
        },
        {
          Question: "Are there commercials? And can I watch on demand?",
          Answer:
            "Apple Originals are always commercial-free. Some shows release all episodes at once. Other shows add new episodes every Friday. You can then watch them on demand anytime, anywhere.",
          isShow: false,
        },
        {
          Question: "Do I need an Apple TV 4K?",
          Answer:
            "No, you don’t. While Apple TV 4K — with 4K HDR and Dolby Atmos sound — is the ultimate way to experience Apple TV+, the original shows and movies on Apple TV+ are always available on the Apple TV app on your favorite devices.",
          isShow: false,
        },
        {
          Question: "Can I download to watch offline?",
          Answer:
            "Absolutely. Download your favorite Apple Originals to your Apple device and watch them anywhere, anytime without a Wi-Fi connection.",
          isShow: false,
        },
      ],
    };
  },
  methods: {},
};
</script>
    
  <style lang="scss" scoped>
$bordercolor: #d2d2d7;
$colorwhite: #fff;
$colorblack: #000;
$tran-opacity: opacity 0;
$opacity: 0;
$button-padding-top: 1em;
$button-padding-bottom: 1em;
.section {
  display: flex;
  flex-direction: column;
  justify-content: center;
  margin-left: auto;
  margin-right: auto;
  .typography-app-headline {
    font-weight: 700;
    text-align: center;
    margin-bottom: 52px;
    font-size: 70px;
    line-height: 1.0555555556;
    font-weight: 700;
    letter-spacing: -0.012em;
    font-family: SF Pro Display, SF Pro Icons, Helvetica Neue, Helvetica, Arial,
      sans-serif;
  }
  .list {
    display: flex;
    flex-direction: column;
    justify-content: center;
    margin-left: auto;
    margin-right: auto;
    width: 91%;
    border-top: solid 1px $bordercolor;
    text-align: justify;
  }
  .list:first-child {
    border-width: 0;
  }

  .collapsible {
    border: none;
    text-align: left;
    outline: none;
    display: flex;
    justify-content: space-between;
    align-items: baseline;
    width: 100%;
    position: relative;
    background-color: $colorwhite;
    color: $colorblack;
    cursor: pointer;
    padding-top: $button-padding-top;
    padding-bottom: $button-padding-bottom;
  }

  .btn {
    font-size: 24px;
    line-height: 1.1666666667;
    font-weight: 600;
    letter-spacing: 0.009em;
    font-family: SF Pro Display, SF Pro Icons, Helvetica Neue, Helvetica, Arial,
      sans-serif;
    --accordion-border-color: #d2d2d7;
  }
}

.fade-enter-active,
.fade-leave-active {
  transition: $tran-opacity;
}
.fade-enter, .fade-leave-to /* .fade-leave-active below version 2.1.8 */ {
  opacity: $opacity;
}
</style>