<template>
  <div>
      <h1>Aprendendo Sobre V-model em formulario</h1>
  </div>
  <div>
      <label >
          <input v-model="name" type="text" /> <br>
          Usuario digitou : {{name}}
      </label>
  </div> <hr><br>
  <div>
      <label>Escolha um esporte</label><br>
      <select v-model="sport" >
          <option value="">Escolha</option>
          <option value="futubol">Futebol</option>
          <option value="basquete">Basquete</option>
          <option value="peteca">Petéca</option>
      </select><br><br>
      Usuario escolher : {{sport}}
  </div><hr><br>
  <div>
      Aceita receber email <br>
    <label>
      <input v-model="aceite" type="radio" value="sim" name="aceite">Sim <br>
      <input v-model="aceite" type="radio" value="nao" name="aceite">Não <br>
    </label>
    Escolheu => {{ aceite }}
  </div><hr><br>
  <div>
      Aceita nossos termos <br>
      <label>
          <input v-model="check" type="checkbox" > {{check}}
      </label>
  </div><hr><br>

  <div>
    <h1>Escolha as cores que mais gosta</h1>
    <input v-model="cores" type="checkbox" value="Azul" > Azul <br>
    <input v-model="cores" type="checkbox" value="Amarelo"> Amarelo <br>
    <input v-model="cores" type="checkbox" value="Verde"> Verde <br>
    <input v-model="cores" type="checkbox" value="Preto"> Preto <br>
    <input v-model="cores" type="checkbox" value="Laranja"> Laranja <br>
    <input v-model="cores" type="checkbox" value="Vermelho"> Vermelho <br>
  </div>
  Cores rescolhidas: {{ cores}}
    
</template>

<script>
    export default {
        data(){
            return{
                name:'',
                sport: '',
                aceite: '',
                check: false,
                cores:[],
            };
        }
    }
</script>

<style scoped>

</style>