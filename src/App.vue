<template>
  <div>
    <BaseAlert v-if="showAlert === true" :msg="msg" :msgType=msgType @closeButton="closeButton()" />
  </div>
</template>
<script>

import BaseAlert from "@/components/Base-Alert.vue";

export default {
  components: {BaseAlert},

  name: "App",
  data() {
    return {
      msg:'Cadastro enviado com sucesso!',
      msgType:"success",
      showAlert: true,
    }
  },
  methods:{
    closeButton(){
      this.showAlert = false;
      console.log('closeButton');
    }
  }
};
</script>

<style>

</style>
