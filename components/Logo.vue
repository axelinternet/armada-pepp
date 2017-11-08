<template>
  <div class="ArmadaLogoHolder">
    <img src="http://armada.nu/assets/logo.png" class="mainLogo" />
  </div>
</template>

<style>
.ArmadaLogoHolder {
  display: inline-block;
  position: relative;
  height: 180px;
  width: 245px;
}


.mainLogo {
  height: auto;
  width: inherit;
}
@keyframes turn {
  100% {
    transform: rotateX(0deg);
  }
}

@keyframes godown {
  100% {
    top: 180px;
  }
}

@keyframes goright {
  100% {
    left: 70px;
  }
}
</style>
