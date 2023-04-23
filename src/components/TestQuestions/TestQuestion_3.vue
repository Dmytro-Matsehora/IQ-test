<script>
  export default {
    name: 'TestQuestion_3',
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
      Выберите лишнее:
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
      Дом
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
      Шалаш
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
      Бунгало
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
      Скамейка
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
      Хижина
    </label>
  </form>
</template>

<style>
</style>