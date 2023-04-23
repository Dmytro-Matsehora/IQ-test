<script>
  export default {
    name: 'TestQuestion_9',
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
      Выберите правильную фигуру из четырёх пронумерованных:
    </h1>

    <img 
      class="question__image"
      src="../../assets/TQ-8_image.svg" 
      alt="question__image"
    >
    
    <div class="question__square-container">
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
        1
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
        2
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
        3
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
        4
      </label>
    </div>
  </form>
</template>

<style lang="scss">
  .question {
    &__square-container {
      margin-top: 26px;
    }  

    &__little-square {
      display: flex;
      justify-content: center;
      align-items: center;
      width: 41px;
      height: 41px;
      box-sizing: border-box;
      background: #FFFFFF;
      font-family: 'PT Serif';
      font-style: normal;
      font-weight: 400;
      font-size: 20px;
      line-height: 49px;
      text-align: center;
      text-transform: capitalize;
      color: #0D0C11;
    }

    &__radio-little-square {
      display: none;
    }

    &__radio-little-square:checked + &__little-square {
      border: 6px solid #FFC700;
    }
  }
</style>