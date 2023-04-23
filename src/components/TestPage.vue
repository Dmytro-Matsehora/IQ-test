<script>
  import TestQuestion_1 from './TestQuestions/TestQuestion_1.vue';
  import TestQuestion_2 from './TestQuestions/TestQuestion_2.vue';
  import TestQuestion_3 from './TestQuestions/TestQuestion_3.vue';
  import TestQuestion_4 from './TestQuestions/TestQuestion_4.vue';
  import TestQuestion_5 from './TestQuestions/TestQuestion_5.vue';
  import TestQuestion_6 from './TestQuestions/TestQuestion_6.vue';
  import TestQuestion_7 from './TestQuestions/TestQuestion_7.vue';
  import TestQuestion_8 from './TestQuestions/TestQuestion_8.vue';
  import TestQuestion_9 from './TestQuestions/TestQuestion_9.vue';
  import TestQuestion_10 from './TestQuestions/TestQuestion_10.vue';
  import TestQuestion_11 from './TestQuestions/TestQuestion_11.vue';
  import TestQuestion_Loader from './TestQuestions/TestQuestion_Loader.vue';

  export default {
    name: 'TestPage',
    components: {
      TestQuestion_1,
      TestQuestion_2,
      TestQuestion_3,
      TestQuestion_4,
      TestQuestion_5,
      TestQuestion_6,
      TestQuestion_7,
      TestQuestion_8,
      TestQuestion_9,
      TestQuestion_10,
      TestQuestion_11,
      TestQuestion_Loader,
    },
    props: {
      page: Number
    },
    data() {
      return {
        buttonDisabled: true,
        progress: 8,
      };
    },
    computed: {
      progressBarWidth() {
        return `${this.progress}%`;
      }
    },
    methods: {
      togglePage() {
        this.$emit('toggle-page');
        this.buttonDisabled = true;
        this.progress += 8;
      },
      buttonDisable() {
        this.buttonDisabled = false;
      }
    }
  }
</script>

<template>
  <div class="question-container">
    <div class="progress-bar">
      <div class="progress-bar__fill" :style="{ width: progressBarWidth }">
      </div>
    </div>

    <TestQuestion_1 
      v-if="page === 1"
      @buttonDisable="buttonDisable"
    />

    <TestQuestion_2 
      v-if="page === 2"
      @buttonDisable="buttonDisable"
    />

    <TestQuestion_3 
      v-if="page === 3"
      @buttonDisable="buttonDisable"
    />
    
    <TestQuestion_4 
      v-if="page === 4"
      @buttonDisable="buttonDisable"
    />

    <TestQuestion_5 
      v-if="page === 5"
      @buttonDisable="buttonDisable"
    />

    <TestQuestion_6 
      v-if="page === 6"
      @buttonDisable="buttonDisable"
    />

    <TestQuestion_7 
      v-if="page === 7"
      @buttonDisable="buttonDisable"
    />

    <TestQuestion_8 
      v-if="page === 8"
      @buttonDisable="buttonDisable"
    />

    <TestQuestion_9 
      v-if="page === 9"
      @buttonDisable="buttonDisable"
    />

    <TestQuestion_10 
      v-if="page === 10"
      @buttonDisable="buttonDisable"
    />

    <TestQuestion_11 
      v-if="page === 11"
      @buttonDisable="buttonDisable"
    />

    <TestQuestion_Loader 
      v-if="page === 12"
      @toggle-page="togglePage"
    />

    <button 
      v-if="page < 12"
      class="button-next" 
      :disabled="buttonDisabled"
      @click="togglePage"
    >
      Далее
    </button>
  </div>
</template>

<style lang="scss">
  .question-container {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
    height: calc(100vh - 48px - 70px);
    background-image: url(../assets/rain_bk2.svg);
  }

  .progress-bar {
    width: 260px;
    height: 11px;
    margin: 17px 0;
    background-color: rgba(242, 243, 243, 0.59);
    mix-blend-mode: normal;
    border-radius: 10.5px;

    &__fill {
      z-index: 2;
      height: 100%;
      background: #3BDE7C;
      border-radius: 10.5px;
    }
  }
  
  .button-next {
    min-height: 41px;
    width: 189px;
    height: 41px;
    background: radial-gradient(50% 50% at 50% 50%, #FFC700 0%, #FFC700 100%);
    color: #0D0C11;
    box-shadow: inset 0px 4px 10px rgba(0, 0, 0, 0.25);
    border-radius: 20px;
    font-family: 'Merriweather';
    font-style: normal;
    font-weight: 700;
    font-size: 14px;
    line-height: 18px;
    text-align: center;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    margin: 25px 0 25px;
    border: none;
    cursor: pointer;

    &:disabled {
      background: #DADADA;
      color: #8E8E8E;
    }
  }
</style>