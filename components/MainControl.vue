<template>
  <div>
    <b-sidebar id="sidebar-right" right visible no-header>
      <div class="px-3 py-4">
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
            <b-form-group
              id="input-group-4"
              label="Necklaces:"
              label-for="input-4"
            >
              <b-form-select
                id="input-4"
                v-model="form.necklaces"
                :options="necklaces_options"
                required
              ></b-form-select>
            </b-form-group>
            <b-form-group
              id="input-group-5"
              label="Eyemakeup:"
              label-for="input-5"
            >
              <b-form-select
                id="input-5"
                v-model="form.eyemakeup"
                :options="eyemakeup_options"
                required
              ></b-form-select>
            </b-form-group>

            <b-form-group
              id="input-group-6"
              label="Piercings:"
              label-for="input-6"
            >
              <b-form-select
                id="input-6"
                v-model="form.piercings"
                :options="piercings_options"
                required
              ></b-form-select>
            </b-form-group>

            <b-form-group
              id="input-group-7"
              label="Piercings:"
              label-for="input-7"
            >
              <b-form-select
                id="input-7"
                v-model="form.facemarkings"
                :options="facemarkings_options"
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
      necklaces_options: [
        { text: "Select One", value: null },
        {
          text: "BUNNYNECKTIE",
          value: "/images/necklaces/BUNNYNECKTIE.png",
        },
        {
          text: "CHAIN",
          value: "/images/necklaces/CHAIN.png",
        },
        {
          text: "CHAINGOLD",
          value: "/images/necklaces/CHAINGOLD.png",
        },
        {
          text: "CHOKER",
          value: "/images/necklaces/CHOKER.png",
        },
        {
          text: "CHOKERBLACK",
          value: "/images/necklaces/CHOKERBLACK.png",
        },
        {
          text: "CHOKERBLACKONELOOP",
          value: "/images/necklaces/CHOKERBLACKONELOOP.png",
        },
        {
          text: "CHOKERBLACKRING",
          value: "/images/necklaces/CHOKERBLACKRING.png",
        },
        {
          text: "CHOKERBLACKTWOLOOPS",
          value: "/images/necklaces/CHOKERBLACKTWOLOOPS.png",
        },
        {
          text: "CHOKERPINK",
          value: "/images/necklaces/CHOKERPINK.png",
        },
        {
          text: "CHOKERRED",
          value: "/images/necklaces/CHOKERRED.png",
        },
        {
          text: "CHOKEWHITE",
          value: "/images/necklaces/CHOKERWHITE.png",
        },
        {
          text: "LONGNECKLACES",
          value: "/images/necklaces/LONGNECKLACES.png",
        },
        {
          text: "NONECKLACES",
          value: "/images/necklaces/NONECKLACES.png",
        },
        {
          text: "ROPE",
          value: "/images/necklaces/ROPE.png",
        },
        {
          text: "SHORTNECKLACES",
          value: "/images/necklaces/SHORTNECKLACES.png",
        },
        {
          text: "THREENECKLACES",
          value: "/images/necklaces/THREENECKLACES.png",
        },
        {
          text: "TWOENECKLACES",
          value: "/images/necklaces/TWONECKLACES.png",
        },
      ],
      eyemakeup_options: [
        { text: "Select One", value: null },
        {
          text: "BULLSEYE",
          value: "/images/eyemakeup/BULLSEYE.png",
        },
        {
          text: "CATEYE",
          value: "/images/eyemakeup/CATEYE.png",
        },
        {
          text: "HEARTCHEEKS",
          value: "/images/eyemakeup/HEARTCHEEKS.png",
        },
        {
          text: "JOKEREYEBLACK",
          value: "/images/eyemakeup/JOKEREYEBLACK.png",
        },
        {
          text: "JOKEREYERED",
          value: "/images/eyemakeup/JOKEREYERED.png",
        },
        {
          text: "KISSONTHECHEEK",
          value: "/images/eyemakeup/KISSONTHECHEEK.png",
        },
        {
          text: "NOMAKEUP",
          value: "/images/eyemakeup/NOMAKEUP.png",
        },
        {
          text: "OUTLINE",
          value: "/images/eyemakeup/OUTLINE.png",
        },
        {
          text: "RACOONEYES",
          value: "/images/eyemakeup/RACOONEYES.png",
        },
        {
          text: "SMOKYEYES",
          value: "/images/eyemakeup/SMOKYEYES.png",
        },
        {
          text: "STARMAKEUP",
          value: "/images/eyemakeup/STARMAKEUP.png",
        },
        {
          text: "WINK",
          value: "/images/eyemakeup/WINK.png",
        },
      ],
      piercings_options: [
        { text: "Select One", value: null },
        {
          text: "NOPIERCINGS",
          value: "/images/piercings/NOPIERCINGS.png",
        },
        {
          text: "NOSTRIL",
          value: "/images/piercings/NOSTRIL.png",
        },
        {
          text: "SEPTUM",
          value: "/images/piercings/SEPTUM.png",
        },
        {
          text: "SIDELABARETE",
          value: "/images/piercings/SIDELABARETE.png",
        },
      ],
      facemarkings_options: [
        { text: "Select One", value: null },
        {
          text: "BEAUTYMARK",
          value: "/images/facemarkings/BEAUTYMARK.png",
        },
        {
          text: "FRECKLES",
          value: "/images/facemarkings/FRECKLES.png",
        },
        {
          text: "HEARTTATTOO",
          value: "/images/facemarkings/HEARTTATTOO.png",
        },
        {
          text: "KATVOND",
          value: "/images/facemarkings/KATVOND.png",
        },
        {
          text: "LIPBEAUTYMARK",
          value: "/images/facemarkings/LIPBEAUTYMARK.png",
        },
        {
          text: "NOFACEMARK",
          value: "/images/facemarkings/NOFACEMARK.png",
        },
        {
          text: "SPRINKLES",
          value: "/images/facemarkings/SPRINKLES.png",
        },
        {
          text: "TEARTATTOO",
          value: "/images/facemarkings/TEARTATTOO.png",
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
