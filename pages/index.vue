<template>
  <div>
    <MainNav />
    <MainControl />
    <b-img
      style="height: calc(100vh - 56px)"
      id="background"
      class="background"
      center
      src="/images/background/RED.png"
      alt="Center image"
    ></b-img>

    <b-img
      style="height: calc(100vh - 56px)"
      id="shadow"
      class="shadow"
      center
      src="/images/shadow/BLOODSPLATTER.png"
      alt="Center image"
    ></b-img>

    <b-img
      style="height: calc(100vh - 56px)"
      id="body"
      class="body"
      center
      src="/images/body/EASYTIGER.png"
      alt="Center image"
    ></b-img>

    <b-img
      style="height: calc(100vh - 56px)"
      id="face"
      class="face"
      center
      src="/images/face/BUSHYEYEBROWS.png"
      alt="Center image"
    ></b-img>
  </div>
</template>

<script>
export default {};
</script>
<style>
.background {
  position: absolute;
  z-index: 1;
}

.shadow {
  position: absolute;

  z-index: 2;
}

.body {
  position: absolute;

  z-index: 3;
}

.face {
  position: absolute;

  z-index: 4;
}
</style>
