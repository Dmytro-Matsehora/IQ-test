<script>
  export default {
    name: 'TestQuestion_10',
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
      Какое определение, по-Вашему, больше подходит к этому геометрическому изображению:
    </h1>

    <img 
      class="question__image"
      src="../../assets/TQ-10_image.svg" 
      alt="question__image"
    >
      
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
      Оно остроконечное
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
      Оно устойчиво
    </label>

    <input 
      type="radio" 
      name="radio" 
      class="question__radio-button" 
      id="checkbox_3"
    >
    <label
      class="question__option" 
      for="checkbox_3" 
      @click="buttonDisable"
    > 
      Оно находится в состоянии равновесия
    </label>
  </form>
</template>

<style>
</style>