<template>
  <div v-bind:class="registerStyle">
    <div class="container">
      <div class="contents">
        <div class="keicon">
          <img class="paSrc" @click="jump(item)" />
        </div>

        <div class="keicon">
          <img
            src="../assets/kf/whatsapp.png"
            class="paSrc"
            v-if="1"
            @click="jumptoWhatsapp('+855968509332')"
          />
          <img
            src="../assets/kf/skype.png"
            class="paSrc"
            v-if="1"
            @click="jumptoAppSkype('vLsdqypFErgL')"
          />
          <img
            src="../assets/kf/telegram.png"
            class="paSrc"
            v-if="1"
            @click="jumptoAppTelegram('+855968509332')"
          />
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  methods: {
    // Whatsapp
    jumptoWhatsapp(val) {
      window.open("https://wa.me/" + val, "_blank");
    },
    // Skype
    jumptoAppSkype(val) {
      window.open("https://join.skype.com/invite/" + val, "_blank");
    },
    // Telegram
    jumptoAppTelegram(val) {
      window.open("https://t.me/" + val, "_blank");
    },
  },
};
</script>
