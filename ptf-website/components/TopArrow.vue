<template>
  <div class="container__topArrow none-topArrow">
    <a href="#section__landingSection" class="anchor__topArrow">
      <p href="#section__landingSection" class="icon__topArrow"></p>
    </a>
  </div>
</template>

<style scoped>
.container__topArrow {
  height: 60px;
  width: 60px;
  opacity: 0.7;

  position: fixed;
  bottom: 1%;
  right: 2%;

  background-color: white;

  border: 3px rgb(69, 69, 69) solid;
  border-radius: 20%;

  z-index: 2;
}

.icon__topArrow {
  border: solid black;
  border-width: 0 5px 5px 0;
  display: inline-block;
  padding: 10px;

  transform: rotate(-135deg);
  -webkit-transform: rotate(-135deg);
}

.anchor__topArrow {
  display: flex;
  align-items: center;
  justify-content: center;

  width: 100%;
  height: 100%;
  padding-top: 5px;
}

.show-topArrow {
  opacity: 1;
}

.none-topArrow {
  opacity: 0;
}

.pop-in {
  animation: pop-in 1s;
}

.pop-out {
  animation: pop-out 1s;
}

@keyframes pop-in {
  from {
    opacity: 0;
    transform: translatey(150px);
  }

  to {
    opacity: 1;
    transform: translatey(0);
  }
}

@keyframes pop-out {
  from {
    opacity: 1;
    transform: translatey(0);
  }


  to {
    opacity: 0;
    transform: translatey(150px);
  }
}</style>

