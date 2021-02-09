<template>
<div class="page_container">
  <div class="content_container">
    <p class="intro"> THINGS I HAVE DONE </p>
    <div class="banner">
      <div class="slide">
        <h2> EXHIBIT A </h2>
      </div>
      <div class="slide">
        <h2> EXHIBIT B </h2>
      </div>
      <div class="slide ">
        <h2> EXHIBIT C </h2>
      </div>
    </div>
    <div class="banner">
      <div class="slide">
        <h2> EXHIBIT D </h2>
      </div>
      <div class="slide">
        <h2> EXHIBIT E </h2>
      </div>
      <div class="slide">
        <h2> EXHIBIT F </h2>
      </div>
    </div>
    <div class="banner">
      <div class="slide">
        <h2> EXHIBIT G </h2>
      </div>
      <div class="slide">
        <h2> EXHIBIT H </h2>
      </div>
      <div class="slide">
        <h2> EXHIBIT I </h2>
      </div>
    </div>
    <div class="footer">
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
</script>

<style (scoped)>
.banner {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-between;
  width: 750px;
  height: 250px;
  margin-top: 10px;
}

.footer {
  width: 800px;
  height: 180px;
}

.slide {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  border: solid 1px;
  height: 100%;
  width: 32.5%;
  background: white;
  transition: transform .4s; 

}

.slide:hover {
  font-weight: bold;
    background-image: url("https://thumbs.gfycat.com/UnsungWindingCuttlefish-size_restricted.gif");
    background-size: contain;
background-position: fixed;
background-repeat: no-repeat;
  color: blue;
}

.salvo {
}

.salvo:hover {
  background-image: url("https://data.whicdn.com/images/316556551/original.gif");
  background-size: contain;
background-position: fixed;
background-repeat: no-repeat;
  color: orange;
}

.empathy{
  
}

.empathy:hover {
  background-image: url("https://i.gifer.com/3Bwl.gif");
  background-size: contain;
  color: red;
}

.alice {
  
}

.alice:hover {
  background-image: url("https://data.whicdn.com/images/302999086/original.gif");
  background-size: fit;
}

.human_mech {
  
}

.human_mech:hover {
  background-image: url("https://thumbs.gfycat.com/UnsungWindingCuttlefish-size_restricted.gif");
    background-size: contain;
background-position: fixed;
background-repeat: no-repeat;
  color: blue;
}

.page_container {

}

.content_container {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 100%;
}

.intro {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  font-size: 80px;
  position: sticky;
}
</style>