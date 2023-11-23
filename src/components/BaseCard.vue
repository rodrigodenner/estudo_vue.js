<template>
  <div class="baseCard">
    <h4>Titulo do card</h4>
    <p>"Neque porro quisquam est qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit..."
      "There is no one who loves pain itself, who seeks after it and wants to have it, simply because it is pain..."</p>
  </div>
</template>

<script>
export default {
  data() {
    return {}
  }
}
</script>

<style scoped>

.baseCard{
  max-width: 300px;
  margin: auto;
  height: 400px;
  padding: 10px;
  background-color: aqua;
  border: solid 2px black;
  border-radius: 10%;
}
h4{
  font-weight: bold;
  text-align: center;
}

</style>