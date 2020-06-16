<template>
  <div class="logo-wrapper">
    <div
      :class="{
        'logo-inner': true,
        blink: blinking
      }"
    >
      <img src="@/assets/uploads/logo_all.png"/>
    </div>
  </div>
</template>
<script>
export default {
  name: 'SiteLogo',
  data() {
    return {
      frames: 5,
      currentFrame: 1,
      blinking: true
    }
  }
}
</script>
<style lang="scss">
.logo-wrapper {
  position: relative;
  height: 100px;
  overflow: hidden;
  width: 300px;
  .logo-inner {
    position: absolute;
    height: 500px;
    img {
      display: block;
      height: 90px;
      margin: 5px;
      max-height: initial;
    }
  }
}
</style>
