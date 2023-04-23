<script>
  export default {
    name: 'TestQuestion_2',
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
      Укажите ваш возраст:
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
      До 18
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
      От 18 до 28
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
      От 29 до 35
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
      От 36
    </label>
  </form>
</template>

<style>
</style>