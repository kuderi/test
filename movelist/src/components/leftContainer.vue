<template>
    <div id="left">
      <div id="box">
        <p v-for="(Fruit, index) in leftFruits" :key="index">{{ Fruit }}</p>
      </div>
      <button @click="moveToRight">右へ移動</button>
    </div>
</template>

<script>
  import { mapState, mapActions } from "vuex";
  export default {
    computed: mapState({
      leftFruits: state => state.leftFruits
    }),
    methods: mapActions(["moveToRight"])
  };
</script>

<style scoped>
#left {
    width: 300px;
    height: 500px;
}

#box {
    width: 100%;
    height: 100%;
    border: 1px solid navy;
    display: inline-block;
    text-align: center;
}
p {
    width: 80%;
    border-bottom: solid 1px navy;
    margin: 0 auto;
    line-height: 50px;
    display: block;
}

button {
    background-color: navy;
    color: white;
    margin: 30px auto;
    height: 40px;
    width: 150px;
    font-size: 16px;
    cursor: pointer;
    display: block;
    border: none;
}
</style>