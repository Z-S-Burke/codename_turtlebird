<template>
  <div class="page_container">
    <div class="content_container">
      <div id="displayCase" class="title">
        <p>flower</p>
        <p style="color: black">.exe</p>
      </div>
        <button v-on:click="setup"> CLICK </button>
      <div class="display">
        <div class="menu">
          <div class="input">
            <button type="button">Style 1</button>
          </div>
          <div class="input">
            <button type="button">Style 2</button>
          </div>
          <div class="input">
            <button type="button">Style 3</button>
          </div>
          <div class="input">
            <button type="button">Style 4</button>
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
      tam: 450,
      fx: 750,
      fy: 750,
    };
  },
  methods: {
    setup() {
      window.open("https://codepen.io/zsburke/pen/eYBzgVg", "_blank");    
    },
  },
};

/*
var tam = 450;
var fx, fy;

fx = 750;
fy = 750;

function setup() {
  console.log("function called")
  createCanvas(fx, fy, WEBGL);
}

function draw() {
  background(255, 255, 255);

  ambientLight(40, 40, 40);
  pointLight(200, 0, 100, 600, 0, 150);
  pointLight(100, 0, 200, -600, 0, 150);
  pointLight(100, 0, 0, 0, 0, 450);

  rotateZ(frameCount * 0.001);
  rotateX(frameCount * 0.001);
  rotateY(frameCount * 0.001);
  rotateX(mouseY * 0.005);
  rotateY(mouseX * 0.005);

  specularMaterial(250);
  translate(0, 0, 35);
  rotateZ(frameCount * 0.01);
  plane(400, 400);
  translate(0, 0, 20);
  rotateZ(frameCount * 0.01);
  plane(350, 350);
  translate(0, 0, 20);
  rotateZ(frameCount * 0.01);
  plane(300, 300);
  translate(0, 0, 20);
  rotateZ(frameCount * 0.01);
  plane(250, 250);
  translate(0, 0, 20);
  rotateZ(frameCount * 0.01);
  plane(200, 200);
  translate(0, 0, 20);
  rotateZ(frameCount * 0.01);
  plane(150, 150);
  translate(0, 0, 20);
  rotateZ(frameCount * 0.01);
  plane(100, 100);
  translate(0, 0, 20);
  rotateZ(frameCount * 0.01);
  plane(50, 50);

  translate(0, 0, -150);
  rotateZ(frameCount * -0.1);
  plane(350, 350);
  translate(0, 0, -20);
  rotateZ(frameCount * -0.01);
  plane(300, 300);
  translate(0, 0, -20);
  rotateZ(frameCount * -0.01);
  plane(250, 250);
  translate(0, 0, -20);
  rotateZ(frameCount * -0.01);
  plane(200, 200);
  translate(0, 0, -20);
  rotateZ(frameCount * -0.01);
  plane(150, 150);
  translate(0, 0, -20);
  rotateZ(frameCount * -0.01);
  plane(100, 100);
  translate(0, 0, -20);
  rotateZ(frameCount * -0.01);
  plane(50, 50);

  document.getElementById("displayCase").appendChild(canvas);
}
*/
</script>

<style (scoped)>
.question_text {
  font-weight: bold;
  font-style: italic;
}
.headerPhoto {
  max-width: 100%;
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
.caption_background {
  background-color: rgb(0, 0, 0, 0.25);
}
.bglight {
  background-color: rgba(255, 255, 255, 0.452);
}

.display {
  display: flex;
  flex-direction: column;
  align-items: center;
  height: 75%;
  justify-content: space-between;
  margin-top: 10px;
}

.footer {
  width: 800px;
  height: 180px;
}

.menu {
  width: 100%;
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-between;
  border-bottom: double #2196f3 20px;
  border-left: double #2196f3 20px;
  padding: 10px;
  margin-bottom: 20px;
}

@keyframes spin {
  from {
    transform: rotate(0deg);
  }
  to {
    transform: rotate(360deg);
  }
}

.input {
  background-color: #2196f3;
}

button {
  padding: 10px;
  margin-left: 20px;
  margin-right: 20px;
  background-color: white;
  font-weight: bold;
}

.page_container {
  width: 100%;
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
}

.content_container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-between;
  height: 100%;
  width: 50%;
  border-top: solid 50px #98ee99;
  border-bottom: solid 50px #98ee99;
}

.title {
  display: flex;
  background-color: (255, 255, 255);
  flex-direction: row;
  align-items: center;
  justify-content: center;
  font-size: 80px;
  color: #2196f3;
  border-top: double black 5px;
  border-left: double black 5px;
  margin-top: 20px;
}
</style>