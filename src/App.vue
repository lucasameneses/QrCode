<template>
      <v-col>
        <v-row>
          <vue-qrious :value="text" size="300" />
        </v-row>
        <v-row>
          <v-flex xs8 sm4 md4 lg3>
            <v-text-field
              placeholder="Digite Aqui !!"
              solo
              v-model="text"
            ></v-text-field>
          </v-flex>
        </v-row>
      </v-col>
</template>

<script src="/path/to/qrious.js"></script> 
<script>
import VueQrious from "vue-qrious";
import Qrious from "qrious";
export default {
  name: "App",
  components: {
    VueQrious,
  },
  data: () => ({
    text: "",
  }),
};
</script>
