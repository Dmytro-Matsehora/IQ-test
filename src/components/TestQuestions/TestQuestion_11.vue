<script>
  export default {
    name: 'TestQuestion_11',
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
      src="../../assets/TQ-11_image.svg" 
      alt="question__image"
    >
      
    <div class="question__square-container square-container">
      <input 
        type="radio" 
        name="radio" 
        class="question__radio-little-square" 
        id="checkbox_1"
      >
      <label 
        class="question__little-square" 
        for="checkbox_1" 
        @click="buttonDisable"
      > 
        34
      </label>

      <input 
        type="radio" 
        name="radio" 
        class="question__radio-little-square" 
        id="checkbox_2"
      >
      <label
        class="question__little-square" 
        for="checkbox_2" 
        @click="buttonDisable"
      > 
        36
      </label>

      <input 
        type="radio" 
        name="radio" 
        class="question__radio-little-square" 
        id="checkbox_3"
      >
      <label
        class="question__little-square" 
        for="checkbox_3" 
        @click="buttonDisable"
      >
        53
      </label>

      <input 
        type="radio" 
        name="radio" 
        class="question__radio-little-square" 
        id="checkbox_4"
      >
      <label
        class="question__little-square" 
        for="checkbox_4" 
        @click="buttonDisable"
      >
        44
      </label>

      <input 
        type="radio" 
        name="radio" 
        class="question__radio-little-square" 
        id="checkbox_5"
      >
      <label
        class="question__little-square" 
        for="checkbox_5" 
        @click="buttonDisable"
      >
        66
      </label>

      <input 
        type="radio" 
        name="radio" 
        class="question__radio-little-square" 
        id="checkbox_6"
      >
      <label
        class="question__little-square" 
        for="checkbox_6" 
        @click="buttonDisable"
      >
        42
      </label>
    </div>
  </form>
</template>

<style lang="scss">
  .square-container {
    width: 300px;
  }

  .question__little-square {
    margin-right: 8px;
  }

  .question__little-square:last-child {
    margin-right: 0;
  }
</style>