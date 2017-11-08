<template>
  <div class="ArmadaLogoHolder">
    <img src="http://armada.nu/assets/logo.png" class="mainLogo" />
  </div>
</template>

<style>
.ArmadaLogoHolder {
  display: flex;
  position: relative;
}

.mainLogo {
  height: 245px;
  width: auto;
  margin: auto;
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
