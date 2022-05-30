<template>
  <div>
    <b-sidebar id="sidebar-right" right visible>
      <div class="px-3 py-2">
        <b-container>
          <b-form>
            <b-form-group
              id="input-group-1"
              label="Background:"
              label-for="input-1"
            >
              <b-form-select
                id="input-1"
                v-model="form.background"
                :options="background_options"
                required
              ></b-form-select>
            </b-form-group>
            <b-form-group
              id="input-group-2"
              label="Shadow:"
              label-for="input-2"
            >
              <b-form-select
                id="input-2"
                v-model="form.shadow"
                :options="shadow_options"
                required
              ></b-form-select>
            </b-form-group>
            <b-form-group id="input-group-3" label="Body:" label-for="input-3">
              <b-form-select
                id="input-3"
                v-model="form.body"
                :options="body_options"
                required
              ></b-form-select>
            </b-form-group>
          </b-form>
        </b-container>
      </div>
    </b-sidebar>
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
      hair_options: [
        { text: "Select One", value: null },
        {
          text: "AERIAL",
          value: "/images/hair/AERIAL.png",
        },
        {
          text: "BEACHBUNNYBLACK",
          value: "/images/hair/BEACHBUNNYBLACK.png",
        },
        {
          text: "BEACHBUNNYBLUE",
          value: "/images/hair/BEACHBUNNYBLUE.png",
        },
        {
          text: "BEACHBUNNYRED",
          value: "/images/hair/BEACHBUNNYRED.png",
        },
        {
          text: "BEACHBUNNYWHITE",
          value: "/images/hair/BEACHBUNNYWHITE.png",
        },
        {
          text: "BLACKWAVES",
          value: "/images/hair/BEACHBUNNYBLACKWAVES.png",
        },
        {
          text: "BOB",
          value: "/images/hair/BOB.png",
        },
        {
          text: "BULLETPROOF",
          value: "/images/hair/BULLETPROOF.png",
        },
        {
          text: "CLEANCUT",
          value: "/images/hair/CLEANCUT.png",
        },
        {
          text: "CRAZYHORSEBLACK",
          value: "/images/hair/CRAZYHORSEBLACK.png",
        },
        {
          text: "CRAZYHORSEBLUE",
          value: "/images/hair/CRAZYHORSEBLUE.png",
        },
        {
          text: "CRAZYHORSEGREEN",
          value: "/images/hair/CRAZYHORSEGREEN.png",
        },
        {
          text: "CRAZYHORSEORANGE",
          value: "/images/hair/CRAZYHORSEORANGE.png",
        },
        {
          text: "CRAZYHORSEPINK",
          value: "/images/hair/CRAZYHORSEPINK.png",
        },
        {
          text: "CRAZYHORSEWHITE",
          value: "/images/hair/CRAZYHORSEWHITE.png",
        },
        {
          text: "CRAZYHORSEYELLOW",
          value: "/images/hair/CRAZYHORSEYELLOW.png",
        },
      ],
      hair_options2: [
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
        "CRAZYHORSEBLACK",
        "CRAZYHORSEBLUE",
        "CRAZYHORSEGREEN",
        "CRAZYHORSEORANGE",
        "CRAZYHORSEPINK",
        "CRAZYHORSEWHITE",
        "CRAZYHORSEYELLOW",
        "FRENCHIEBLACK",
        "FRENCHIERED",
        "GIJANE",
        "GREYBERETTE",
        "HARFLIP",
        "HARLERYQ",
        "HELMET",
        "HELMETHAIR",
        "LANABLACK",
        "LANARED",
        "LANAWHITE",
        "MERMAIDDARK",
        "MERMAIDWHITE",
        "MESSY",
        "MESSYBUN",
        "MESSYWETHAIR",
        "MICKEYMOUSECLUB",
        "PIGTAILS",
        "QUINNPIGTAILS",
        "RAGDOLLPIGTAILS",
        "REDBERETTE",
        "REDBUNS",
        "REDWAVES",
        "REGAL",
        "STASSI",
        "WETHAIR",
        "WHITEBUNS",
        "WHITEWAVES",
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
      background_options: [
        { text: "Select One", value: null },
        {
          text: "GREY",
          value: "/images/background/GREY.png",
        },
        {
          text: "RED",
          value: "/images/background/RED.png",
        },
        {
          text: "REDSPOTLIGHT",
          value: "/images/background/REDSPOTLIGHT.png",
        },
        {
          text: "WHITEPOTLIGHT",
          value: "/images/background/WHITEPOTLIGHT.png",
        },
        {
          text: "WHITE",
          value: "/images/background/WHITE.png",
        },
      ],
      shadow_options: [
        { text: "Select One", value: null },
        {
          text: "BLOODSPLATTER",
          value: "/images/shadow/BLOODSPLATTER.png",
        },
        {
          text: "DEVILTAIL",
          value: "/images/shadow/DEVILTAIL.png",
        },
        {
          text: "NOSHADOW",
          value: "/images/shadow/NOSHADOW.png",
        },
        {
          text: "THEDEVILYOUKNOW",
          value: "/images/shadow/THEDEVILYOUKNOW.png",
        },
      ],
      body_options: [
        { text: "Select One", value: null },
        {
          text: "ATLANTIS",
          value: "/images/body/ATLANTIS.png",
        },
        {
          text: "AVATAR",
          value: "/images/body/AVATAR.png",
        },
        {
          text: "BANGBANG",
          value: "/images/body/BANGBANG.png",
        },
        {
          text: "BASEBALLRIFFLE",
          value: "/images/body/BASEBALLRIFFLE.png",
        },
        {
          text: "BATTERUP",
          value: "/images/body/BATTERUP.png",
        },
        {
          text: "BAZUCA",
          value: "/images/body/BAZUCA.png",
        },
        {
          text: "BLACKLIGHTER",
          value: "/images/body/BLACKLIGHTER.png",
        },
        {
          text: "BLACKLONGSLV",
          value: "/images/body/BLACKLONGSLV.png",
        },
        {
          text: "BLACKMONEYGUN",
          value: "/images/body/BLACKMONEYGUN.png",
        },
        {
          text: "BLOODYHELL",
          value: "/images/body/BLOODYHELL.png",
        },
        {
          text: "BULLETPROOF",
          value: "/images/body/BULLETPROOF.png",
        },
        {
          text: "BURNTHEEVIDENCE",
          value: "/images/body/BURNTHEEVIDENCE.png",
        },
        {
          text: "BURNTHEHOUSEDOWN",
          value: "/images/body/BURNTHEHOUSEDOWN.png",
        },
        {
          text: "DEALERSCHOICE",
          value: "/images/body/DEALERSCHOICE.png",
        },
        {
          text: "DESTINATIONHEIST",
          value: "/images/body/DESTINATIONHEIST.png",
        },
        {
          text: "DOMINATRIX",
          value: "/images/body/DOMINATRIX.png",
        },
        {
          text: "EASYTIGER",
          value: "/images/body/EASYTIGER.png",
        },
        {
          text: "FINEACCESORY",
          value: "/images/body/FINEACCESORY.png",
        },
        {
          text: "FIRSTDATE",
          value: "/images/body/FIRSTDATE.png",
        },
        {
          text: "GLOVESWITHLIPSTICK",
          value: "/images/body/GLOVESWITHLIPSTICK.png",
        },
        {
          text: "GODSAVETHEQUEEN",
          value: "/images/body/GODSAVETHEQUEEN.png",
        },
        {
          text: "GOTTHEMONEY",
          value: "/images/body/GOTTHEMONEY.png",
        },
        {
          text: "GREYBLAZER",
          value: "/images/body/GREYBLAZER.png",
        },
        {
          text: "HARNESS",
          value: "/images/body/HARNESS.png",
        },
        {
          text: "HARNESSTHEPOWER",
          value: "/images/body/HARNESSTHEPOWER.png",
        },
      ],
      show: true,
    };
  },

  watch: {
    form: {
      deep: true,
      handler() {
        this.$emit("form", this.form);
      },
    },
  },
};
</script>
