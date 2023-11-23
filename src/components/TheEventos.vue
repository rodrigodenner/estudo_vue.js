<template>
    <div>
      <h1>Evento de Click</h1> 
      <button @click="onClick">
        Enviar
      </button>
    </div><br><br>
    <div>
      <h1>Formulario </h1>
      <form 
      action="https://google.com"
      @submit.prevent ="onSubmit"
      >

      <button type="submit">
        enviar
      </button>
      </form>
    </div>
</template>

<script>
export default {
  data(){
    return{

    }
  },
  methods:{
    onClick(){
      alert('Clicou');
    },
    onSubmit(){
      console.log('Submit');
    }
  }

}
</script>

<style scoped>

</style>