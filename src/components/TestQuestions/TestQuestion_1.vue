<script>
  export default {
    name: 'TestQuestion_1',
    methods: {
      buttonDisable() {
        this.$emit('button-disable');
      }
    }
  }
</script>

<template>
  <form class="question">
    <h1 class="question__title">
      Ваш пол:
    </h1>
      
    <input 
      type="radio" 
      name="radio" 
      class="question__radio-button" 
      id="checkbox_1"
    >
    <label 
      class="question__option" 
      for="checkbox_1" 
      @click="buttonDisable"
    > 
      Мужчина 
    </label>

    <input 
      type="radio" 
      name="radio" 
      class="question__radio-button" 
      id="checkbox_2"
    >
    <label 
      class="question__option" 
      for="checkbox_2" 
      @click="buttonDisable"
    > 
      Женщина 
    </label>
  </form>
</template>

<style lang="scss">
</style>