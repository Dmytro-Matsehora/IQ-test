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
      Вам привычнее и важнее:
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
      Наслаждаться каждой минутой проведенного времени
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
      Быть устремленными мыслями в будущее
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
      Учитывать в ежедневной практике прошлый опыт
    </label>
  </form>
</template>

<style>
</style>