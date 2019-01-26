<template>
  <div
    class="button-native"
    @click="emitClickEvent"
  >
    <span>
      {{ label }}
    </span>
  </div>
</template>

<style>
  .button-native {
    min-width: 193px;
    height: 50px;
    border-radius: 25px;
    background: #57b846;
    font-family: Montserrat;
    font-weight: 800;
    font-size: 15px;
    line-height: 1.5;
    color: #fff;
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 0 25px;
    cursor: pointer;
  }
</style>

<script>
  export default {
    props: {
      label: {
        type: String,
        required: true
      }
    },
    methods: {
      emitClickEvent() {
        this.$emit('click')
      }
    }
  }
</script>