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
            <b-form-group id="input-group-5" label="Faces:" label-for="input-5">
              <b-form-select
                id="input-5"
                v-model="form.face"
                :options="faces_options"
                required
              ></b-form-select>
            </b-form-group>
            <b-form-group
              id="input-group-6"
              label="Eyemakeup:"
              label-for="input-6"
            >
              <b-form-select
                id="input-6"
                v-model="form.eyemakeup"
                :options="eyemakeup_options"
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
                v-model="form.piercings"
                :options="piercings_options"
                required
              ></b-form-select>
            </b-form-group>

            <b-form-group
              id="input-group-8"
              label="Facemarkings:"
              label-for="input-8"
            >
              <b-form-select
                id="input-8"
                v-model="form.facemarkings"
                :options="facemarkings_options"
                required
              ></b-form-select>
            </b-form-group>

            <b-form-group
              id="input-group-9"
              label="Lipstick:"
              label-for="input-9"
            >
              <b-form-select
                id="input-9"
                v-model="form.lipstick"
                :options="lipstick_options"
                required
              ></b-form-select>
            </b-form-group>

            <b-form-group
              id="input-group-10"
              label="Mouthcoverings:"
              label-for="input-10"
            >
              <b-form-select
                id="input-10"
                v-model="form.mouthcoverings"
                :options="mouthcoverings_options"
                required
              ></b-form-select>
            </b-form-group>

            <b-form-group
              id="input-group-11"
              label="Sunglasses:"
              label-for="input-11"
            >
              <b-form-select
                id="input-11"
                v-model="form.sunglasses"
                :options="sunglasses_options"
                required
              ></b-form-select>
            </b-form-group>

            <b-form-group
              id="input-group-12"
              label="Hair:"
              label-for="input-12"
            >
              <b-form-select
                id="input-12"
                v-model="form.hair"
                :options="hair_options"
                required
              ></b-form-select>
            </b-form-group>

            <b-form-group
              id="input-group-12"
              label="Over the head:"
              label-for="input-13"
            >
              <b-form-select
                id="input-13"
                v-model="form.overthehead"
                :options="overthehead_options"
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

      background_options: [
        { text: "Select one", value: null },
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
        { text: "Select one", value: null },
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
        { text: "Select one", value: null },
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
        { text: "Select one", value: null },
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
          text: "Select oneCKLACES",
          value: "/images/necklaces/Select oneCKLACES.png",
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
      faces_options: [
        { text: "Select one", value: null },
        {
          text: "BUSHYEYEBROWS",
          value: "/images/face/BUSHYEYEBROWS.png",
        },
        {
          text: "MANICUREDBROWS",
          value: "/images/face/MANICUREDBROWS.png",
        },
      ],
      eyemakeup_options: [
        { text: "Select one", value: null },
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
        { text: "Select one", value: null },
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
        { text: "Select one", value: null },
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
      lipstick_options: [
        { text: "Select one", value: null },
        {
          text: "BEAUTYMARK",
          value: "/images/lipstick/BUBBLEGUM.png",
        },
        {
          text: "BURGUNDYBULLET",
          value: "/images/lipstick/BURGUNDYBULLET.png",
        },
        {
          text: "BURGUNDYCIGAR",
          value: "/images/lipstick/BURGUNDYCIGAR.png",
        },
        {
          text: "BURGUNDYCIGARETTE",
          value: "/images/lipstick/BURGUNDYCIGARETTE.png",
        },
        {
          text: "BURGUNDYGROWL",
          value: "/images/lipstick/BURGUNDYGROWL.png",
        },
        {
          text: "BURGUNDYHAPPY",
          value: "/images/lipstick/BURGUNDYGROWL.png",
        },
        {
          text: "BURGUNDYMATCHES",
          value: "/images/lipstick/BURGUNDYMATCHES.png",
        },
        {
          text: "BURGUNDYVAMP",
          value: "/images/lipstick/BURGUNDYVAMP.png",
        },
        {
          text: "GREYGROWL",
          value: "/images/lipstick/GREYGROWL.png",
        },
        {
          text: "LIPKIT",
          value: "/images/lipstick/LIPKIT.png",
        },
        {
          text: "LIPKITMATCHES",
          value: "/images/lipstick/LIPKITMATCHES.png",
        },
        {
          text: "PILLOWTALK",
          value: "/images/lipstick/PILLOWTALK.png",
        },
        {
          text: "PILLOWTALKCIGAR",
          value: "/images/lipstick/PILLOWTALKCIGAR.png",
        },
        {
          text: "PILLOWTALKCIGARETTE",
          value: "/images/lipstick/PILLOWTALKCIGARETTE.png",
        },
        {
          text: "PILLOWTALKGROWL",
          value: "/images/lipstick/PILLOWTALKGROWL.png",
        },
        {
          text: "PILLOWTALKHAPPY",
          value: "/images/lipstick/PILLOWTALKHAPPY.png",
        },
        {
          text: "PILLOWTALKMATCHES",
          value: "/images/lipstick/PILLOWTALKMATCHES.png",
        },
        {
          text: "REDBULLET",
          value: "/images/lipstick/REDBULLET.png",
        },
        {
          text: "REDGROWL",
          value: "/images/lipstick/REDGROWL.png",
        },
        {
          text: "REDLIPS",
          value: "/images/lipstick/REDLIPS.png",
        },
        {
          text: "REDVAMP",
          value: "/images/lipstick/REDVAMP.png",
        },
        {
          text: "SHINYRED",
          value: "/images/lipstick/SHINYRED.png",
        },
        {
          text: "SHINYREDCIGAR",
          value: "/images/lipstick/SHINYREDCIGAR.png",
        },
        {
          text: "SHINYREDCIGAR",
          value: "/images/lipstick/SHINYREDCIGAR.png",
        },
        {
          text: "SHINYREDCIGARETTE",
          value: "/images/lipstick/SHINYREDCIGARETTE.png",
        },
        {
          text: "SHINYREDHAPPY",
          value: "/images/lipstick/SHINYREDHAPPY.png",
        },
        {
          text: "SHINYREDMATCHES",
          value: "/images/lipstick/SHINYREDMATCHES.png",
        },
        {
          text: "SIREN",
          value: "/images/lipstick/SIREN.png",
        },
        {
          text: "SIRENGROWL",
          value: "/images/lipstick/SIRENGROWL.png",
        },
        {
          text: "SIRENMATCHES",
          value: "/images/lipstick/SIRENMATCHES.png",
        },
        {
          text: "TAUPEBULLET",
          value: "/images/lipstick/TAUPEBULLET.png",
        },
        {
          text: "TAUPECIGAR",
          value: "/images/lipstick/TAUPECIGAR.png",
        },
        {
          text: "TAUPECIGARETTE",
          value: "/images/lipstick/TAUPECIGARETTE.png",
        },
        {
          text: "TAUPEHAPPY",
          value: "/images/lipstick/TAUPEHAPPY.png",
        },
        {
          text: "TAUPEMATCHES",
          value: "/images/lipstick/TAUPEMATCHES.png",
        },
      ],
      mouthcoverings_options: [
        { text: "Select one", value: null },
        {
          text: "BANDANABLACK",
          value: "/images/mouthcoverings/BANDANABLACK.png",
        },
        {
          text: "BANDANAGREY",
          value: "/images/mouthcoverings/BANDANAGREY.png",
        },
        {
          text: "BANDANARED",
          value: "/images/mouthcoverings/BANDANARED.png",
        },
        {
          text: "BLOODYLIP",
          value: "/images/mouthcoverings/BLOODYLIP.png",
        },
        {
          text: "FACEMASK",
          value: "/images/mouthcoverings/FACEMASK.png",
        },
        {
          text: "NOMOUTHCOVERING",
          value: "/images/mouthcoverings/NOMOUTHCOVERING.png",
        },
      ],
      sunglasses_options: [
        { text: "Select one", value: null },
        {
          text: "AVIATOR",
          value: "/images/sunglasses/AVIATOR.png",
        },
        {
          text: "BLUEHEARTS",
          value: "/images/sunglasses/BLUEHEARTS.png",
        },
        {
          text: "CATEYE",
          value: "/images/sunglasses/CATEYE.png",
        },
        {
          text: "CLEARGLASSES",
          value: "/images/sunglasses/CLEARGLASSES.png",
        },
        {
          text: "CLEARPINK",
          value: "/images/sunglasses/CLEARPINK.png",
        },
        {
          text: "FUTURE",
          value: "/images/sunglasses/FUTURE.png",
        },
        {
          text: "HARRY-POTTER",
          value: "/images/sunglasses/HARRY-POTTER.png",
        },
        {
          text: "NOGLASSES",
          value: "/images/sunglasses/NOGLASSES.png",
        },
        {
          text: "PINKHEARTS",
          value: "/images/sunglasses/PINKHEARTS.png",
        },
        {
          text: "PIRATE",
          value: "/images/sunglasses/PIRATE.png",
        },
        {
          text: "SPARKLER",
          value: "/images/sunglasses/SPARKLER.png",
        },
        {
          text: "VINTAGE",
          value: "/images/sunglasses/VINTAGE.png",
        },
      ],
      hair_options: [
        { text: "Select one", value: null },
        {
          text: "ARIEL",
          value: "/images/hair/ARIEL.png",
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
        {
          text: "FRENCHIEBLACK",
          value: "/images/hair/FRENCHIEBLACK.png",
        },
        {
          text: "FRENCHIERED",
          value: "/images/hair/FRENCHIERED.png",
        },
        {
          text: "GIJANE",
          value: "/images/hair/GIJANE.png",
        },
        {
          text: "GREYBERETTE",
          value: "/images/hair/GREYBERETTE.png",
        },
        {
          text: "HAIRFLIP",
          value: "/images/hair/HAIRFLIP.png",
        },
        {
          text: "HARLEYQ",
          value: "/images/hair/HAIRFLIP.png",
        },
        {
          text: "HELMET",
          value: "/images/hair/HELMET.png",
        },
        {
          text: "HELMETHAIR",
          value: "/images/hair/HELMETHAIR.png",
        },
        {
          text: "LANABLACK",
          value: "/images/hair/LANABLACK.png",
        },
        {
          text: "LANARED",
          value: "/images/hair/LANARED.png",
        },
        {
          text: "LANAWHITE",
          value: "/images/hair/LANAWHITE.png",
        },
        {
          text: "MERMAIDDARK",
          value: "/images/hair/MERMAIDDARK.png",
        },
        {
          text: "MERMAIDWHITE",
          value: "/images/hair/MERMAIDWHITE.png",
        },
        {
          text: "MESSY",
          value: "/images/hair/MESSY.png",
        },
        {
          text: "MESSY",
          value: "/images/hair/MESSY.png",
        },
        {
          text: "MESSYBUN",
          value: "/images/hair/MESSYBUN.png",
        },
        {
          text: "MESSYWETHAIR",
          value: "/images/hair/MESSYWETHAIR.png",
        },
        {
          text: "MICKEYMOUSECLUB",
          value: "/images/hair/MICKEYMOUSECLUB.png",
        },
        {
          text: "PIGTAILS",
          value: "/images/hair/PIGTAILS.png",
        },
        {
          text: "QUINNPIGTAILS",
          value: "/images/hair/QUINNPIGTAILS.png",
        },
        {
          text: "RAGDOLLPIGTAILS",
          value: "/images/hair/RAGDOLLPIGTAILS.png",
        },
        {
          text: "REDBERETTE",
          value: "/images/hair/REDBERETTE.png",
        },
        {
          text: "REDBUNS",
          value: "/images/hair/REDBUNS.png",
        },
        {
          text: "REDWAVES",
          value: "/images/hair/REDWAVES.png",
        },
        {
          text: "REGAL",
          value: "/images/hair/REGAL.png",
        },
        {
          text: "STASSI",
          value: "/images/hair/STASSI.png",
        },
        {
          text: "WETHAIR",
          value: "/images/hair/WETHAIR.png",
        },
        {
          text: "WHITEBUNS",
          value: "/images/hair/WHITEBUNS.png",
        },
        {
          text: "WHITEWAVES",
          value: "/images/hair/WHITEWAVES.png",
        },
      ],

      overthehead_options: [
        { text: "Select one", value: null },
        {
          text: "HALO",
          value: "/images/overthehead/HALO.png",
        },
        {
          text: "NOHALO",
          value: "/images/overthehead/NOHALO.png",
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
