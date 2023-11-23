<template>
  <div>
    <input v-model="name" type="text" /> <br>
    {{name}}
  </div> <br><br>

  <select v-model="pageCount">
    <option value="5">5</option>
    <option value="10">10</option>
    <option value="15">15</option>
  </select><br><br>
  Pagina - {{pageCount}}


</template>

<script>
export default {
  data() {
    return {
      name: '',
      pageCount: 5
    }
  },
  watch:{
    name(vl){
      if(vl.length >=3){
        this.saveUserName()
      }
    },
    pageCount(){
      this.changePage();  
      if(this.pageCount == 15){
        this.alertView();
      }
      
    }
    
  },
  computed:{
    
  },

  methods:{
    saveUserName(){
      console.log('Ajax');
      console.log(this.name);
    },
    changePage(){
      console.log('Ajax');
      console.log('Valor enviado');
    },
    alertView(){
      alert('Você clicou em 15');
    }

  }

}
</script>

<style >

</style>