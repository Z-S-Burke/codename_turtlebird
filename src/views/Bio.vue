<template>
  <div>
    <div v-if="mobileCheck()">
      <div class="content_container">
        <p class="intro">THINGS I HAVE DONE</p>
        <div class="mobileBanner">
          <div class="mobileSlide">
            <h2>EXHIBIT A</h2>
          </div>
          <div class="mobileSlide">
            <h2>EXHIBIT B</h2>
          </div>
          <div v-on:click="setup" class="mobileSlide">
            <h2>flower.exe</h2>
          </div>
          <div class="mobileSlide">
            <h2>EXHIBIT D</h2>
          </div>
          <div class="mobileSlide">
            <h2>EXHIBIT E</h2>
          </div>
          <div class="mobileSlide">
            <h2>EXHIBIT F</h2>
          </div>
          <div class="mobileSlide">
            <h2>EXHIBIT G</h2>
          </div>
          <div class="mobileSlide">
            <h2>EXHIBIT H</h2>
          </div>
        </div>
      </div>
    </div>
    <div v-if="!mobileCheck()">
      <div class="content_container">
        <p class="intro">THINGS I HAVE DONE</p>
        <div class="banner">
          <div class="slide">
            <h2>EXHIBIT A</h2>
          </div>
          <div class="slide">
            <h2>EXHIBIT B</h2>
          </div>
          <div v-on:click="setup" class="flower flowerText">
            <h2>flower.exe</h2>
          </div>
          <div class="slide">
            <h2>EXHIBIT D</h2>
          </div>
          <div class="slide">
            <h2>EXHIBIT E</h2>
          </div>
          <div class="slide">
            <h2>EXHIBIT F</h2>
          </div>
          <div class="slide">
            <h2>EXHIBIT G</h2>
          </div>
          <div class="slide">
            <h2>EXHIBIT H</h2>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      /* eslint-disable */
      slide: 0,
      sliding: null,
      mobile: false,
    };
  },
  created: {
    function() {
      this.mobileCheck();
    },
  },
  methods: {
    setup() {
      window.open("https://codepen.io/zsburke/pen/eYBzgVg", "_blank");
    },
    mobileCheck() {
      if (window.innerWidth <= 760) {
        this.mobile = true;
      }
      return this.mobile;
    },
  },
};
</script>

<style (scoped)>
.banner {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  align-items: center;
  justify-content: space-between;
  width: 90%;
  height: 250px;
  margin-top: 10px;
}

.mobileBanner {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: around;
  width: 90%;
  height: 90%;
}

.slide {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  border: solid 1px;
  height: 100%;
  width: 20%;
  transition: transform 0.4s;
  margin-top: 15px;
  margin-bottom: 15px;
}

.mobileSlide {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  border: solid 1px;
  height: 250px;
  width: 100%;
  transition: transform 0.4s;
  margin-top: 15px;
  margin-bottom: 15px;  
}

.flower {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  border: solid 1px;
  height: 100%;
  width: 20%;
  margin-left: 1px;
  margin-right: 1px;
  background-color: white;
  transition: transform 0.4s;
}


.flower:hover {
  background-image: url("https://i.gifer.com/MaEZ.gif");
  background-repeat: no-repeat;
  background-size: contain;
  color: aquamarine;
}

.flowerText {
  background-color: white;
  padding: 10px;
}

.slide:hover {
  font-weight: bold;
  background-image: url("https://thumbs.gfycat.com/UnsungWindingCuttlefish-size_restricted.gif");
  background-size: cover;
  background-position: fixed;
  background-repeat: no-repeat;
  color: blue;
}

.content_container {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 100vw;
}

.intro {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  font-size: 80px;
  position: sticky;
  background-color: #2196f3;
  font-family: Impact;
  width: 100%;
}
</style>