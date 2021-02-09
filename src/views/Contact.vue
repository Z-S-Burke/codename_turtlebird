<template>
  <div class="bglight splash_image">

  </div>
</template>

<script>
export default {
  data() {
    return {
      /* eslint-disable */
      slide: 0,
      sliding: null
    };
  },
  methods: {
    onSlideStart(slide) {
      this.sliding = true;
    },
    onSlideEnd(slide) {
      this.sliding = false;
    }
  }
};
</script>

<style (scoped)>
.question_text {
  font-weight: bold;
  font-style: italic;
}
.headerPhoto {
  max-width: 100%;
}
.contactDiv {
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  font-size: 1.2em;
  border-bottom: inset;
}
.carousel_border {
  border-style: double;
  border-color: white;
  border-width: 10px;
  padding: 10px;
}
.icon_style {
  height: 20%;
  width: 20%;
  margin: 10px;
}
.iconText {
  margin-right: 20px;
}
@media screen and (min-width: 500px) {
  .carousel_border {
    border-width: 50px;
    padding: 25px;
  }
}
.caption_background {
  background-color: rgb(0, 0, 0, 0.25);
}
.bglight {
  background-color: rgba(255, 255, 255, 0.452);
}
</style>