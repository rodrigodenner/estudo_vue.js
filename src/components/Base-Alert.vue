<template>
  <div :class="['alert', msgType ]" >
    <p>{{msg}}</p>
    <button @click="onClick()">
      x
    </button>

  </div>
</template>

<script>
export default {
  props:{
    msg: String,
    msgType: String,
  },
  methods:{
    onClick(){
      this.$emit('closeButton');
    }
  },
}
</script>

<style  scoped>

.alert{
  padding: 2px;
  border-radius: 6px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 300px;
}

.danger{
  background-color: #fcbaba;
  color: #980000;
}

.success{
  background-color: #7bf17b;
  color: green;
}
button{
  width: 20px;
  height: 20px;
  margin-right: 5px;
  background-color: #ccccf6;
  padding: 1px;

}
</style>