<script>
  export default {
    name: 'TestQuestion_7',
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
      Какой из городов лишний?
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
      Вашингтон
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
      Лондон
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
      Париж
    </label>

    <input 
      type="radio" 
      name="radio" 
      class="question__radio-button" 
      id="checkbox_4"
    >
    <label
      class="question__option" 
      for="checkbox_4" 
      @click="buttonDisable"
    > 
      Нью-Йорк
    </label>

    <input 
      type="radio" 
      name="radio" 
      class="question__radio-button" 
      id="checkbox_5"
    >
    <label
      class="question__option" 
      for="checkbox_5" 
      @click="buttonDisable"
    > 
      Москва
    </label>

    <input 
      type="radio" 
      name="radio" 
      class="question__radio-button" 
      id="checkbox_6"
    >
    <label
      class="question__option" 
      for="checkbox_6" 
      @click="buttonDisable"
    > 
      Оттава
    </label>
  </form>
</template>

<style>
</style>