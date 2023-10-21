<template>
  <div>
    <h2>Lista de Usuários</h2>

    <div v-for="todo in todos" v-bind:key=todo.id>
        <div v-if="todo.imgSrc">
            Olá {{ todo.fullName}}
            <img v-bind:src="todo.imgSrc" :alt="todo.imgAlt" >
            <hr>
        </div> 
        <div v-else>
        Olá {{ todo.fullName }} <br><br> Que pena voce está sem foto <br>
        <a href="">Adicionar foto</a>
        </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {

      todos: [
        {
          "userId": 1,
          "id": 1,
          "fullName": "Rodrigo Denner",
          "imgSrc":'https://static.vecteezy.com/ti/vetor-gratis/t2/4607791-cara-de-homem-emotiva-icone-sorridente-personagem-masculino-de-camisa-azul-ilustracao-isolado-no-branco-feliz-humano-psicologico-retrato-emocoes-positivas-usuario-avatar-para-app-web-design-vetor.jpg',
          "imgAlt":"Foto aleatoria"
        },
        {
          "userId": 1,
          "id": 1,
          "fullName": "Francisco Denner",
          "imgSrc":"https://static.vecteezy.com/ti/vetor-gratis/t2/2002403-homem-com-barba-avatar-personagem-icone-isolado-gratis-vetor.jpg",
          "imgAlt":"Foto aleatoria"
        },
        
      ],
    };
  }
};
</script>