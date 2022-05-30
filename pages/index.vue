<template>
  <div style="background-color: #000 !important; height: 100vh">
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
        id="necklaces"
        class="necklaces"
        center
        :src="form.necklaces"
      ></b-img>

      <b-img
        style="height: calc(100vh - 56px)"
        id="face"
        class="face"
        center
        :src="form.face"
      ></b-img>

      <b-img
        style="height: calc(100vh - 56px)"
        id="eyemakeup"
        class="eyemakeup"
        center
        :src="form.eyemakeup"
      ></b-img>

      <b-img
        style="height: calc(100vh - 56px)"
        id="piercings"
        class="piercings"
        center
        :src="form.piercings"
      ></b-img>
      <b-img
        style="height: calc(100vh - 56px)"
        id="facemarkings"
        class="facemarkings"
        center
        :src="form.facemarkings"
      ></b-img>

      <b-img
        style="height: calc(100vh - 56px)"
        id="lipstick"
        class="lipstick"
        center
        :src="form.lipstick"
      ></b-img>

      <b-img
        style="height: calc(100vh - 56px)"
        id="mouthcoverings"
        class="mouthcoverings"
        center
        :src="form.mouthcoverings"
      ></b-img>

      <b-img
        style="height: calc(100vh - 56px)"
        id="sunglasses"
        class="sunglasses"
        center
        :src="form.sunglasses"
      ></b-img>

      <b-img
        style="height: calc(100vh - 56px)"
        id="hair"
        class="hair"
        center
        :src="form.hair"
      ></b-img>

      <b-img
        style="height: calc(100vh - 56px)"
        id="overthehead"
        class="overthehead"
        center
        :src="form.overthehead"
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

.necklaces {
  position: absolute;

  z-index: 4;
}

.face {
  position: absolute;

  z-index: 5;
}
.eyemakeup {
  position: absolute;

  z-index: 6;
}

.piercings {
  position: absolute;

  z-index: 7;
}
.facemarkings {
  position: absolute;

  z-index: 8;
}

.lipstick {
  position: absolute;

  z-index: 9;
}

.mouthcoverings {
  position: absolute;

  z-index: 10;
}

.sunglasses {
  position: absolute;

  z-index: 11;
}

.hair {
  position: absolute;

  z-index: 12;
}

.overthehead {
  position: absolute;

  z-index: 13;
}
</style>
