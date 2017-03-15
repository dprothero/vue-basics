<template lang="pug">
#app
  qrcode(v-bind:cls="qrCls", v-vbind:value="qrText")
</template>

<script>
const Qrcode = require('v-qrcode');

module.exports = {
  name: 'app',
  data() {
    return {
      qrCls: 'qrcode',
      qrText: 'hello world'
    }
  },
  components: {
    Qrcode
  }
};
</script>
