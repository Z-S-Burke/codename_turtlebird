<template>
  <div class="bglight splash_image">
    <div class="m-3 text-left text-dark carousel_border textBoxStyle">
      <h4 class="textHeader text-center py-5">Javier Pérez Sandoval</h4>
      <ul class="p-3">
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quisque
          placerat ultricies justo a lobortis. Proin ac suscipit sem. Ut
          dignissim vitae ante ac scelerisque. Nullam ut nisi ligula. Etiam
          malesuada et risus ut consequat. In eros erat, interdum nec tempus
          eget, faucibus ac urna. Curabitur tempus placerat sodales.
        </p>
        <p>
Sed vehicula porta risus non gravida. Etiam et rhoncus lacus. Aliquam nisi mauris, tincidunt nec lectus quis, tempor molestie metus. Duis pulvinar nunc nec leo pharetra, sit amet convallis tortor imperdiet. Cras vel imperdiet libero. Vestibulum vitae mollis dolor. In mattis, mi quis interdum vulputate, ipsum risus malesuada arcu, ut pretium mauris velit ut dolor. Ut condimentum, nunc id facilisis vestibulum, enim mauris pulvinar dui, blandit sodales sapien velit non purus. Curabitur eget euismod lacus.
        </p>
        <p>
Nunc pharetra, enim in interdum egestas, metus nisi placerat velit, at viverra dolor nulla sit amet sapien. In hac habitasse platea dictumst. Suspendisse potenti. Cras tincidunt eros lectus. Praesent ornare nibh ante, eu porta ligula vestibulum placerat. Etiam commodo tortor sapien, vel malesuada leo sagittis eget. Sed cursus velit quis nunc cursus sagittis. Aliquam maximus elit quis sem pharetra maximus. Morbi arcu ipsum, volutpat sit amet malesuada sit amet, scelerisque non lectus. Nunc metus dolor, pulvinar in fringilla sit amet, convallis pulvinar tortor. Nulla at mauris laoreet, porttitor justo at, ullamcorper diam. Interdum et malesuada fames ac ante ipsum primis in faucibus.
        </p>
        <p>
Sed vehicula porta risus non gravida. Etiam et rhoncus lacus. Aliquam nisi mauris, tincidunt nec lectus quis, tempor molestie metus. Duis pulvinar nunc nec leo pharetra, sit amet convallis tortor imperdiet. Cras vel imperdiet libero. Vestibulum vitae mollis dolor. In mattis, mi quis interdum vulputate, ipsum risus malesuada arcu, ut pretium mauris velit ut dolor. Ut condimentum, nunc id facilisis vestibulum, enim mauris pulvinar dui, blandit sodales sapien velit non purus. Curabitur eget euismod lacus.
        </p>
        <p>
Sed vehicula porta risus non gravida. Etiam et rhoncus lacus. Aliquam nisi mauris, tincidunt nec lectus quis, tempor molestie metus. Duis pulvinar nunc nec leo pharetra, sit amet convallis tortor imperdiet. Cras vel imperdiet libero. Vestibulum vitae mollis dolor. In mattis, mi quis interdum vulputate, ipsum risus malesuada arcu, ut pretium mauris velit ut dolor. Ut condimentum, nunc id facilisis vestibulum, enim mauris pulvinar dui, blandit sodales sapien velit non purus. Curabitur eget euismod lacus.
        </p>
        <p>
Sed vehicula porta risus non gravida. Etiam et rhoncus lacus. Aliquam nisi mauris, tincidunt nec lectus quis, tempor molestie metus. Duis pulvinar nunc nec leo pharetra, sit amet convallis tortor imperdiet. Cras vel imperdiet libero. Vestibulum vitae mollis dolor. In mattis, mi quis interdum vulputate, ipsum risus malesuada arcu, ut pretium mauris velit ut dolor. Ut condimentum, nunc id facilisis vestibulum, enim mauris pulvinar dui, blandit sodales sapien velit non purus. Curabitur eget euismod lacus.
        </p>
      </ul>
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
    };
  },
  methods: {
    onSlideStart(slide) {
      this.sliding = true;
    },
    onSlideEnd(slide) {
      this.sliding = false;
    },
  },
};
</script>

<style (scoped)>
.question_text {
  font-weight: bold;
  font-style: italic;
}
.carousel_border {
  border-style: double;
  border-color: white;
  border-width: 10px;
  padding: 10px;
}
@media screen and (min-width: 500px) {
  .carousel_border {
    border-width: 50px;
    padding: 25px;
  }
}
.headerPhoto {
  padding: 10%;
  max-width: 100%;
}
.caption_background {
  background-color: rgb(0, 0, 0, 0.25);
}
.bglight {
  background-color: rgba(255, 255, 255, 0.452);
}

.textHeader {
  background-color: #2196f3;
}

.textBoxStyle {
  background-color: white;
}
</style>