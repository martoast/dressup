<template>
  <div>
    <MainNav />
    <MainControl @form="onFormUpdate" />
    <div class="parent">
      <b-img
        style="height: calc(100vh - 56px)"
        id="background"
        class="background"
        center
        :src="form.background"
      ></b-img>

      <b-img
        style="height: calc(100vh - 56px)"
        id="shadow"
        class="shadow"
        center
        :src="form.shadow"
      ></b-img>

      <b-img
        style="height: calc(100vh - 56px)"
        id="body"
        class="body"
        center
        :src="form.body"
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
  </div>
</template>

<script>
export default {
  data() {
    return {
      form: {
        background: null,
        shadow: null,
        body: null,
        necklaces: null,
        face: null,
        eyemakeup: null,
        piercings: null,
        facemarkings: null,
        lipstick: null,
        mouthcoverings: null,
        sunglasses: null,
        hair: null,
        overthehead: null,
      },
    };
  },
  methods: {
    onFormUpdate(form) {
      this.form = form;
      console.log(this.form);
    },
  },
};
</script>
<style>
.parent {
  position: relative;
  display: block;
  margin-left: auto;
  margin-right: auto;
  width: 50%;
}
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
