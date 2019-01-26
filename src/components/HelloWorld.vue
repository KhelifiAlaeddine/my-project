<template>
  <my-button :label="label" @click="animate()"/>
</template>

<script>
import myButton from "./my-button.vue";

export default {
  components: {
    myButton
  },
  data() {
    return {
      label: "Click here"
    };
  },
    methods: {
      animate () {
        alert("here")
      }
    }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
