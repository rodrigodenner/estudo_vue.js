<template>
  <div>

  </div>
</template>

<script>
export default {
  data () {
    return {
      name:"Rodrigo denner"
    }
  },
  //antes de criar o componente
  beforeCreate(){
    
    console.log('antes de criar o componente',this.name);
  },
  //criando o componente
  created() {
    
    console.log('criando o componente',this.name);
  },
  //depois criar o componente
  beforeMount() {
    
    console.log('depois de criar o  componente',this.name);
  },
  //componente montado
  mounted() {
    
    console.log('componente montado ',this.name);
  },
  // //antes de desmontar o componente
  // beforeUnmount() {
  //   console.log('antes de desmontar o  componente');
  // },
  // //deletando o componente
  // unmounted() {
  //   console.log('deletando o componente');
  // },
  watch:{

  },
  computed:{

  },
  methods: {
    
  },
}
</script>

<style scoped>

</style>