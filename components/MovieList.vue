<template>
  <div class="container">
    <div class="movie_card_container">
      <div v-for="(movie, i) of movies_1" :key="i">
        <img :src="movie.img" class="movie_card" />
      </div>
    </div>
    <div class="movie_card_container" id="movie_list_2">
      <div v-for="(movie, i) of movies_2" :key="i">
        <img :src="movie.img" class="movie_card" />
      </div>
    </div>

    <div class="see_full_container">
      <div></div>
      <span>See full lineup ></span>
      <img
        class="icon"
        src="https://www.apple.com/v/apple-tv-plus/ag/images/overview/controls/play_icon__d0s6k3q8dzu6_large.svg"
      />
    </div>
  </div>
</template>
  
  <script>
export default {
  name: "MovieList",
  data: () => ({
    movies_1: [
      {
        img: "https://images.hdqwalls.com/download/mt-st-helens-washington-5k-7u-378x217.jpg",
      },
      {
        img: "https://images.hdqwalls.com/download/artistic-3d-shapes-4k-abstract-q7-378x217.jpg",
      },
      {
        img: "https://images.hdqwalls.com/download/swirls-of-abstract-4k-hk-378x217.jpg",
      },
      {
        img: "https://images.hdqwalls.com/download/3d-color-blend-bubble-4k-ic-378x217.jpg",
      },
      {
        img: "https://images.hdqwalls.com/download/glitch-abstract-5k-gz-378x217.jpg",
      },
      {
        img: "https://images.hdqwalls.com/download/swirl-digital-abstract-4k-9a-378x217.jpg",
      },
      {
        img: "https://images.hdqwalls.com/download/3d-abstract-digital-art-shapes-nq-378x217.jpg",
      },
    ],
    movies_2: [
      {
        img: "https://images.hdqwalls.com/download/3d-cinema-landscape-hs-378x217.jpg",
      },
      {
        img: "https://images.hdqwalls.com/download/deer-landscape-manipulation-mountains-sun-rising-rz-378x217.jpg",
      },
      {
        img: "https://images.hdqwalls.com/download/deer-digtial-vector-art-5k-gk-378x217.jpg",
      },
      {
        img: "https://images.hdqwalls.com/download/deer-antler-silhouette-ar-378x217.jpg",
      },
      {
        img: "https://images.hdqwalls.com/download/cat-and-butterfly-uw-378x217.jpg",
      },
      {
        img: "https://images.hdqwalls.com/download/zoy-lofi-cat-5k-ba-378x217.jpg",
      },
      {
        img: "https://images.hdqwalls.com/download/cat-synthwave-tq-378x217.jpg",
      },
    ],
  }),

  mounted() {
    // let flag = true;
    // setInterval(() => {
    //   let content = document.querySelector(".movie_card_container");
    //   if (flag) content.scrollLeft += 1;
    //   else content.scrollLeft -= 1;
    //   if (content.scrollLeft > 850) {
    //     flag = false;
    //   } else if (content.scrollLeft == 0) {
    //     flag = true;
    //   }
    // }, 10);
    let content = document.querySelector("#movie_list_2");
    content.scrollLeft += 200;
  },
};
</script>
  
  <style lang="scss" scoped>
.container {
  background-color: #000;
  padding: 10px 0 20px 0;
  .movie_card_container {
    display: flex;
    justify-content: space-between;
    overflow-x: hidden;
    @media only screen and (min-width: 1px) {
      .movie_card {
        height: 100px;
        padding: 3px 7px !important;
      }
    }
    @media only screen and (min-width: 425px) {
      .movie_card {
        height: 130px;
      }
    }
    @media only screen and (min-width: 720px) {
      .movie_card {
        height: 180px;
      }
    }
    @media only screen and (min-width: 1280px) {
      .movie_card {
        height: 200px;
      }
    }
    .movie_card {
      border-radius: 15px;
      padding: 10px 10px;
    }
  }

  .see_full_container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0 3rem;
    span {
      color: white;
      border: 1px solid white;
      padding: 10px 20px;
      margin: 20px 0;
      border-radius: 20px;
    }
    .icon {
      width: 36px;
      height: 36px;
    }
  }
}
</style>