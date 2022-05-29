<template>
  <div>
    <b-container>
      <b-form>
        <b-form-group id="input-group-1" label="Hair:" label-for="input-1">
          <b-form-select
            id="input-1"
            v-model="form.hair"
            :options="hair_options"
            required
          ></b-form-select>
        </b-form-group>
        <b-form-group id="input-group-2" label="Eyes:" label-for="input-2">
          <b-form-select
            id="input-2"
            v-model="form.eyes"
            :options="eye_options"
            required
          ></b-form-select>
        </b-form-group>
        <b-form-group id="input-group-3" label="Lipstick:" label-for="input-3">
          <b-form-select
            id="input-3"
            v-model="form.lipstick"
            :options="lipstick_options"
            required
          ></b-form-select>
        </b-form-group>
      </b-form>
    </b-container>
  </div>
</template>

<script>
export default {
  data() {
    return {
      form: {
        background: null,
        face: null,
        hair: null,
        eyes: null,
        lipstick: null,
      },
      hair_options: [
        { text: "Select One", value: null },
        "AERIAL",
        "BEACHBUNNYBLACK",
        "BEACHNUNNYBLUE",
        "BEACHNUNNYRED",
        "BEACHNUNNYWHITE",
        "BLACKWAVES",
        "BOB",
        "BULLETPROOF",
        "CLEANCUT",
        "CRAZYHORSE",
      ],
      eye_options: [
        { text: "Select One", value: null },
        "Carrots",
        "Beans",
        "Tomatoes",
        "Corn",
      ],
      lipstick_options: [
        { text: "Select One", value: null },
        "Carrots",
        "Beans",
        "Tomatoes",
        "Corn",
      ],
      show: true,
    };
  },

  watch: {
    form: {
      deep: true,
      handler() {
        console.log(this.form);
        this.$emit("form", this.form);
      },
    },
  },
};
</script>
