<template>
  <div>
    <b-sidebar id="sidebar-right" title="Controls" right shadow>
      <b-container>
        <b-form @submit="onSubmit" @reset="onReset" v-if="show">
          <b-form-group id="input-group-1" label="Hair:" label-for="input-1">
            <b-form-select
              id="input-1"
              v-model="form.hair"
              :options="hair_options"
              required
            ></b-form-select>
          </b-form-group>
          <b-form-group id="input-group-2" label="Food:" label-for="input-2">
            <b-form-select
              id="input-2"
              v-model="form.eyes"
              :options="eye_options"
              required
            ></b-form-select>
          </b-form-group>
          <b-form-group id="input-group-3" label="Food:" label-for="input-3">
            <b-form-select
              id="input-3"
              v-model="form.mouth"
              :options="mouth_options"
              required
            ></b-form-select>
          </b-form-group>

          <b-button type="submit" variant="primary">Submit</b-button>
          <b-button type="reset" variant="danger">Reset</b-button>
        </b-form>
      </b-container>
    </b-sidebar>
  </div>
</template>

<script>
export default {
  data() {
    return {
      form: {
        hair: null,
        eyes: null,
        mouth: null,
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
      mouth_options: [
        { text: "Select One", value: null },
        "Carrots",
        "Beans",
        "Tomatoes",
        "Corn",
      ],
      show: true,
    };
  },
  methods: {
    onSubmit(event) {
      event.preventDefault();
      alert(JSON.stringify(this.form));
    },
    onReset(event) {
      event.preventDefault();
      // Reset our form values
      this.form.email = "";
      this.form.name = "";
      this.form.food = null;
      this.form.checked = [];
      // Trick to reset/clear native browser form validation state
      this.show = false;
      this.$nextTick(() => {
        this.show = true;
      });
    },
  },
};
</script>
