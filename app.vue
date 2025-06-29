<template>
  <div class="app-background">
    <NuxtPage />
  </div>
</template>

<style scoped>
/* From Uiverse.io by SergeyTwg */
.app-background {
  --gradient-from: #308859;
  --gradient-to: #29312d;
  --bg: #282828;

  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  min-height: 100vh;
  width: 100vw;
  overflow: hidden;
  background: linear-gradient(
    -15deg,
    var(--gradient-to) 0%,
    var(--gradient-from) 70%
  );
  z-index: -1;
}

.app-background:after {
  content: "";
  display: block;
  position: absolute;
  top: -35%;
  height: 200%;
  left: min(-500px, -25%);
  right: min(-500px, -35%);
  overflow: hidden;
  background:
    linear-gradient(
        88.5deg,
        var(--bg) 0%,
        var(--bg) 40%,
        transparent 40%,
        transparent 100%
      )
      0px 0px,
    linear-gradient(
        91.5deg,
        transparent 0%,
        transparent 60%,
        var(--bg) 60%,
        var(--bg) 100%
      )
      0px 0px;
  background-size: 75px 100%;
  transform: rotate(-15deg) skew(15deg, 15deg);
  z-index: -1;
}
</style>
