<template>
  <div class="header">
    <div class="header_tittle">A Space trip from Earth to Mars</div>
    <div class="path">
      <div class="advance_line"></div>
      <div class="steps">
        <div class="step_item"></div>
        <div class="step_item"></div>
        <div class="step_item"></div>
        <div class="step_item"></div>
        <div class="step_item"></div>
      </div>
    </div>
  </div>
</template>


<style>
.header {
  position: fixed;
  left: 0;
  top: 0;
  z-index: 7;
  padding: 16px;
  width: 100%;
  background-color: rgba(16, 16, 16, 0.907);

  display: flex;
  flex-direction: column;
}

.header_tittle {
  font-family: "Roboto";
  color: #cbcbcb;
  margin-bottom: 12px;
}

.path {
  position: relative;

  height: 5px;
  width: 100%;
  background-color: rgb(50, 50, 50);
}

.advance_line {
  height: 5px;
  width: 0;
  background-color: #cbcbcb;
  transition: all 1s ease-out;

  position: absolute;
  top: 0;
  left: 0;
}


.advance_line.perc1{
  width: 25%;
}

.advance_line.perc2{
  width: 50%;
}

.advance_line.perc3{
  width: 75%;
}

.advance_line.perc4{
  width: 100%;
}

.steps {
  position: absolute;
  top: 5px;
  left: 0;
  width: 100%;

  display: flex;
  justify-content: space-between;
}

.step_item {
  height: 5px;
  width: 5px;
  background-color: #cbcbcb;
}
</style>