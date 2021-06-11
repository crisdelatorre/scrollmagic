
<template>
  <div class="app">
    <!-- <Header /> -->
    <!-- BACKGROUND SETUP -->
    <div class="background_setup">
      <div id="c0" class="bg_planets">
        <img class="img_item" src="~/assets/img/bg_planets2.png" alt="" />
      </div>

      <div id="tittle1" class="tittle">
        <h1>54.6 Million Kilometers</h1>
      </div>
    </div>

    <!-- MAIN INFO  -->
    <div class="main_info">
      <div class="entry1 info_left">
        <EntryComponent />
      </div>

      <div class="quote1 info_right">
        <QuoteComponent />
      </div>

      <div class="meteorites">
        <img class="img" src="~/assets/img/meteoritos.png" alt="" />
      </div>

      <div class="entry2 info_right">
        <EntryComponent />
      </div>

      <div class="quote2 info_left">
        <QuoteComponent />
      </div>

      <div class="moon">
        <img class="img2" src="~/assets/img/luna.jpg" alt="" />
      </div>
    </div>

    <!--TIMELINE  -->
    <div class="timeline">
      <div class="line">
        <div class="dots">
          <div class="position_bd dot1">
            <BlueDots />
          </div>
          <div class="position_bd dot2">
            <BlueDots />
          </div>
          <div class="position_gd dot3">
            <GreyDots />
          </div>
          <div class="position_bd dot4">
            <BlueDots />
          </div>
          <div class="position_bd dot5">
            <BlueDots />
          </div>
          <div class="position_gd dot6">
            <GreyDots />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  mounted() {
    const controller = new this.$scrollmagic.Controller();

    var header0 = new this.$scrollmagic.Scene({
      triggerElement: ".tittle",
    })
      .setClassToggle(".advance_line", "perc1")
      // .addIndicators({
      //   name: "line-grow",
      //   colorTrigger: "blue",
      // })
      .addTo(controller);

    var header2 = new this.$scrollmagic.Scene({
      triggerElement: ".dot1",
    })
      .setClassToggle(".advance_line", "perc2")
      // .addIndicators({
      //   name: "line-grow",
      //   colorTrigger: "blue",
      // })
      .addTo(controller);

    var header3 = new this.$scrollmagic.Scene({
      triggerElement: ".dot4",
    })
      .setClassToggle(".advance_line", "perc3")
      // .addIndicators({
      //   name: "line-grow",
      //   colorTrigger: "blue",
      // })
      .addTo(controller);

    var header4 = new this.$scrollmagic.Scene({
      triggerElement: ".dot5",
    })
      .setClassToggle(".advance_line", "perc4")
      // .addIndicators({
      //   name: "line-grow",
      //   colorTrigger: "blue",
      // })
      .addTo(controller);

    var tittleScene = new this.$scrollmagic.Scene({
      triggerElement: ".tittle",
      duration: 350,
    })
      .setClassToggle(".tittle", "fade_in")
      // .addIndicators({
      //   name: "fade-tittle",
      //   colorTrigger: "blue",
      // })
      .addTo(controller);

    var lineScene = new this.$scrollmagic.Scene({
      triggerElement: ".line",
      duration: 1350,
    })
      .setClassToggle(".line", "grow")
      // .addIndicators({
      //   name: "line-grow",
      //   colorTrigger: "blue",
      // })
      .addTo(controller);

    var dot1Scene = new this.$scrollmagic.Scene({
      triggerElement: ".dot1",
      duration: 200,
    })
      .setClassToggle(".dot1", "dot_fade")
      // .addIndicators({
      //   name: "dot-fade",
      //   colorTrigger: "blue",
      // })
      .addTo(controller);

    var entry1Scene = new this.$scrollmagic.Scene({
      triggerElement: ".dot1",
      duration: 200,
    })
      .setClassToggle(".entry1", "fade_in")
      // .addIndicators({
      //   name: "entry1",
      //   colorTrigger: "blue",
      // })
      .addTo(controller);

    var dot2Scene = new this.$scrollmagic.Scene({
      triggerElement: ".dot2",
      duration: 200,
    })
      .setClassToggle(".dot2", "dot_fade")
      // .addIndicators({
      //   name: "dot-fade",
      //   colorTrigger: "blue",
      // })
      .addTo(controller);

    var quote1Scene = new this.$scrollmagic.Scene({
      triggerElement: ".dot2",
      duration: 200,
    })
      .setClassToggle(".quote1", "fade_in")
      // .addIndicators({
      //   name: "quote1",
      //   colorTrigger: "blue",
      // })
      .addTo(controller);

    var dot3Scene = new this.$scrollmagic.Scene({
      triggerElement: ".dot3",
      duration: 200,
    })
      .setClassToggle(".dot3", "dot_fade")
      // .addIndicators({
      //   name: "dot-fade",
      //   colorTrigger: "blue",
      // })
      .addTo(controller);

    var meteoritesScene = new this.$scrollmagic.Scene({
      triggerElement: ".dot3",
      duration: 200,
    })
      .setClassToggle(".meteorites", "fade_in")
      // .addIndicators({
      //   name: "meteorites",
      //   colorTrigger: "blue",
      // })
      .addTo(controller);

    var dot4Scene = new this.$scrollmagic.Scene({
      triggerElement: ".dot4",
      duration: 200,
    })
      .setClassToggle(".dot4", "dot_fade")
      // .addIndicators({
      //   name: "dot-fade",
      //   colorTrigger: "blue",
      // })
      .addTo(controller);

    var entry2Scene = new this.$scrollmagic.Scene({
      triggerElement: ".dot4",
      duration: 200,
    })
      .setClassToggle(".entry2", "fade_in")
      // .addIndicators({
      //   name: "entry2",
      //   colorTrigger: "blue",
      // })
      .addTo(controller);

    var dot5Scene = new this.$scrollmagic.Scene({
      triggerElement: ".dot5",
      duration: 200,
    })
      .setClassToggle(".dot5", "dot_fade")
      // .addIndicators({
      //   name: "dot-fade",
      //   colorTrigger: "blue",
      // })
      .addTo(controller);

    var quote2Scene = new this.$scrollmagic.Scene({
      triggerElement: ".dot5",
      duration: 200,
    })
      .setClassToggle(".quote2", "fade_in")
      // .addIndicators({
      //   name: "quote2",
      //   colorTrigger: "blue",
      // })
      .addTo(controller);

    var dot6Scene = new this.$scrollmagic.Scene({
      triggerElement: ".dot6",
      duration: 200,
    })
      .setClassToggle(".dot6", "dot_fade")
      // .addIndicators({
      //   name: "dot-fade",
      //   colorTrigger: "blue",
      // })
      .addTo(controller);

    var moonScene = new this.$scrollmagic.Scene({
      triggerElement: ".dot6",
      duration: 200,
    })
      .setClassToggle(".moon", "fade_in")
      // .addIndicators({
      //   name: "moon",
      //   colorTrigger: "blue",
      // })
      .addTo(controller);
  },
};
</script>

<style lang="scss">
body {
  color: #bdbdbd;
  background-color: rgb(0, 0, 0);
}

.app {
  position: relative;
}

.bg_planets {
  // height: 100vh;
  height: 100%;
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  img {
    height: 100%;
    width: 100%;
    object-fit: cover;
  }
}

.background_setup {
  background-color: rgb(0, 0, 0);
  width: 100%;
  height: 2000px;
  // position: relative;
}

.tittle {
  font-family: "QTAgateType";
  color: #0ec5ff;
  font-size: 50px;

  position: absolute;
  width: 100%;
  z-index: 3;

  padding: 1rem 1rem;
  text-align: center;
  background-color: rgba(0, 0, 0, 0.775);
  top: 55vh;

  opacity: 0;
  transform: translateY(-15px);
  transition: all 1s ease-out;

  @media (max-width: 1185px) {
    font-size: 30px;
  }

  @media (max-width: 720px) {
    font-size: 20px;
  }
}

.tittle.fade_in {
  opacity: 1;
}

/*
 *  MAIN INFO
 */

.main_info {
  position: absolute;
  z-index: 4;
  top: 102vh;
  left: 10%;

  width: 80%;
  margin: 0 auto;

  display: flex;
  flex-direction: column;
  justify-content: center;
}

.info_left {
  display: flex;
  justify-content: flex-start;
  margin-top: 60px;
}

.info_right {
  display: flex;
  justify-content: flex-end;
  margin-top: 60px;
}

.entry1 {
  opacity: 0;
  transform: translateY(-15px);
  transition: all 1s ease-out;
}

.entry1.fade_in {
  opacity: 1;
}

.quote1 {
  opacity: 0;
  transform: translateY(-15px);
  transition: all 1s ease-out;
}

.quote1.fade_in {
  opacity: 1;
}
.meteorites {
  position: absolute;
  top: 400px;
  left: 0;

  opacity: 0;
  transform: translateY(-15px);
  transition: all 1s ease-out;
}

.meteorites.fade_in {
  opacity: 1;
}

.entry2 {
  opacity: 0;
  transform: translateY(-15px);
  transition: all 1s ease-out;
}

.entry2.fade_in {
  opacity: 1;
}

.quote2 {
  opacity: 0;
  transform: translateY(-15px);
  transition: all 1s ease-out;
}

.quote2.fade_in {
  opacity: 1;
}

.moon {
  height: 15%;
  width: 15%;
  position: absolute;
  bottom: -80px;
  right: 10%;

  opacity: 0;
  transform: translateY(-15px);
  transition: all 1s ease-out;

  img {
    width: 100%;
    height: 100%;

    object-fit: cover;
  }
}

.moon.fade_in {
  opacity: 1;
}

// .links {
//   padding-top: 15px;
// }

.timeline {
  position: absolute;
  top: 80vh;
  left: 50%;
  z-index: 5;
  box-shadow: 8px 8px 16px #1e1e1ea8;

  .line {
    width: 3px;
    height: 0;
    background-color: #0ec5ff;
    transition: height 1s ease-in-out;

    .dots {
      position: absolute;
      // top: 20px;

      .position_bd {
        position: absolute;
        left: -8pt;
      }

      .position_gd {
        position: absolute;
        left: -4pt;
      }
    }
  }
}

.line.grow {
  height: 1200px;
}

.dot {
  opacity: 0;
  transition: opacity 1s ease-out;
}

.dot.dot_fade {
  opacity: 1;
}

.dot1 {
  top: 32vh;
  opacity: 0;
  transition: opacity 1s ease-out;
}

.dot1.dot_fade {
  opacity: 1;
}

.dot2 {
  top: 76vh;
  opacity: 0;
  transition: opacity 1s ease-out;
}

.dot2.dot_fade {
  opacity: 1;
}

.dot3 {
  top: 90vh;
  opacity: 0;
  transition: opacity 1s ease-out;
}

.dot3.dot_fade {
  opacity: 1;
}

.dot4 {
  top: 105vh;
  opacity: 0;
  transition: opacity 1s ease-out;
}

.dot4.dot_fade {
  opacity: 1;
}

.dot5 {
  top: 152vh;
  opacity: 0;
  transition: opacity 1s ease-out;
}

.dot5.dot_fade {
  opacity: 1;
}

.dot6 {
  top: 162vh;
  opacity: 0;
  transition: opacity 1s ease-out;
}

.dot6.dot_fade {
  opacity: 1;
}
</style>
