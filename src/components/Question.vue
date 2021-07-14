<template>
<div>
  <div class="question" @click="toggleShow()">
  <div class="question-number">{{number}}</div>
  <div class="question-string" :class="{'question-h2': isShow}">{{question.question}}</div>
  <div class="detail-button"><i class="fas fa-chevron-down"></i></div>
 </div>
 <div class="answer" v-show="isShow">
    {{question.answer}}
 </div>
</div>
</template>
<script>
export default {
  name: 'Question',
  props: ['number', 'question'],
  data() {
    return {
      isShow: false,
    };
  },
  methods: {
    toggleShow() {
      this.isShow = !this.isShow;
    },
  },
};
</script>
<style>

.question{
     display:flex;
 }

.question-string{
  font-size:14px;
  width:625px;
  margin-right:30px;
}
 .question-h2{
     font-size: 1.5rem;
 }
</style>
