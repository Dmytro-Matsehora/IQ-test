<script>
  export default {
    name: 'TestQuestion_4',
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
      Продолжите числовой ряд: <br>
      18 20 24 32
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
      62
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
      48
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
      74
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
      57
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
      60
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
      77
    </label>
  </form>
</template>

<style>
</style>