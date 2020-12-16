<template>
  <v-col>
    <vue-qrious :value="text" size="300" />
    <barcode :value="text" />
    <v-flex xs8 sm4 md4 lg3>
      <v-text-field
        placeholder="Digite Aqui !!"
        solo
        v-model="text"
      ></v-text-field>
    </v-flex>
  </v-col>
</template>

<script scr src="/path/to/qrious.js"></script> 
<script>
import VueQrious from "vue-qrious";
import Qrious from "qrious";
import VueBarcode from "vue-barcode";
export default {
  name: "App",
  components: {
    VueQrious,
    barcode: VueBarcode,
  },
  data: () => ({
    text: "",
  }),
};
</script>

