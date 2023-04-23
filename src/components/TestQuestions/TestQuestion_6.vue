<script>
  export default {
    name: 'TestQuestion_6',
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
      Отдохните пару секунд, еще раз выберите цвет, который сейчас наиболее Вам приятен:
    </h1>
      
    <div class="question__square-container">
      <input 
        type="radio" 
        name="radio" 
        class="question__radio-square" 
        id="checkbox_1"
      >
      <label 
        class="question__square question__square--grey" 
        for="checkbox_1" 
        @click="buttonDisable"
      > 
      </label>

      <input 
        type="radio" 
        name="radio" 
        class="question__radio-square" 
        id="checkbox_2"
      >
      <label 
        class="question__square question__square--aquamarine" 
        for="checkbox_2" 
        @click="buttonDisable"
      > 
      </label>

      <input 
        type="radio" 
        name="radio" 
        class="question__radio-square" 
        id="checkbox_3"
      >
      <label 
        class="question__square question__square--brown" 
        for="checkbox_3" 
        @click="buttonDisable"
      > 
      </label>

      <input 
        type="radio" 
        name="radio" 
        class="question__radio-square" 
        id="checkbox_4"
      >
      <label 
        class="question__square question__square--green" 
        for="checkbox_4" 
        @click="buttonDisable"
      > 
      </label>

      <input 
        type="radio" 
        name="radio" 
        class="question__radio-square" 
        id="checkbox_5"
      >
      <label 
        class="question__square question__square--black" 
        for="checkbox_5" 
        @click="buttonDisable"
      > 
      </label>

      <input 
        type="radio" 
        name="radio" 
        class="question__radio-square" 
        id="checkbox_6"
      >
      <label 
        class="question__square question__square--red" 
        for="checkbox_6" 
        @click="buttonDisable"
      > 
      </label>

      <input 
        type="radio" 
        name="radio" 
        class="question__radio-square" 
        id="checkbox_7"
      >
      <label 
        class="question__square question__square--purple" 
        for="checkbox_7" 
        @click="buttonDisable"
      > 
      </label>

      <input 
        type="radio" 
        name="radio" 
        class="question__radio-square" 
        id="checkbox_8"
      >
      <label 
        class="question__square question__square--yellow" 
        for="checkbox_8" 
        @click="buttonDisable"
      > 
      </label>

      <input 
        type="radio" 
        name="radio" 
        class="question__radio-square" 
        id="checkbox_9"
      >
      <label 
        class="question__square question__square--blue" 
        for="checkbox_9" 
        @click="buttonDisable"
      > 
      </label>
    </div>
  </form>
</template>

<style lang="scss">
  .question {
    align-items: center;
  }
</style>