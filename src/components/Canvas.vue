<template>
  <div id="canvas"></div>
</template>

<script>
import P5 from "p5"; // Package from npm

export default {
  name: "App",
  mounted() {
    let fx = 750;
    let fy = 750;
    const canvasScript = (p5) => {
      // These are your typical setup() and draw() methods
      p5.setup = () => {
        p5.createCanvas(fx, fy);
      };
      p5.draw = () => {
        p5.background(255, 255, 255);

        p5.ambientLight(40, 40, 40);
        p5.pointLight(200, 0, 100, 600, 0, 150);
        p5.pointLight(100, 0, 200, -600, 0, 150);
        p5.pointLight(100, 0, 0, 0, 0, 450);

        P5(canvasScript, "canvas");
      };
    };
    // Attach the canvas to the div
    P5(canvasScript, "canvas");
  },
};
</script>

<style></style>