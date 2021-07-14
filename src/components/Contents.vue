<template>
   <div class="category-content">
      <div class="category-name">{{selectedCategoryName}}</div>
      <div class="common"><a href="" class="os">os 공통</a></div>
      <div class="question-list">
        <div class="question-item" v-for="(question, number) in selectedQuestionList" :key="number">
          <Question :number="number + 1" :question="question"/>
        </div>
      </div>
      <div class="inquiry">
        <div class="inquiry-text">
          원하시는 답변을 찾지못하셨다면, 고객센터로 문의해 주세요.
        </div>
        <button class="inquiry-button">
          <i class="fas fa-pencil-alt"></i>문의하기
        </button>
      </div>
    </div>
</template>
<script>
import Question from './Question.vue';

export default {
  name: 'Contents',
  props: ['selectedCategoryName', 'selectedQuestionList'],
  components: {
    Question,
  },
};
</script>
<style>
.category-content{
  width:809px;
  border-left:1px solid #e8e8e8;
}

.category-content>div{
  margin-left:58px;
}

.category-name{
  font-size:30px;
  font-weight: bold;
  margin: 40px 0px;
}

.common{
  padding:15px 0px 15px 5px;
  border-top:2px solid black;
}

.os{
  color:black;
  font-size:16px;
  margin:0px 7px;
}

.question-list{
  padding:20px 0px;
  border-top:2px solid black;
  border-bottom:1px solid black;
}

.question-item{
  display:flex;
  padding:15px 0px;
}

.question-item:not(:last-child){
    border-bottom:1px solid #e8e8e8;
}
.question-number{
  font-size:14px;
}

.question-string{
  display:flex;
  margin-left:50px;
  text-decoration: none;
  color:black;
}

/* .question{
  font-size:14px;
  width:625px;
  margin-right:30px;
} */

.detail-button{
  margin:0px 15px 0px auto;
}

.fa-chevron-down{
  font-size:13px;
}

.inquiry{
  display:flex;
  margin-top:40px;
  padding-bottom:100px;
}

.inquiry-text{
  line-height:46px;
  font-size:13px;
}

.inquiry-button{
  border:none;
  margin-left:auto;
  width:186px;
  height:42px;
}

.fa-pencil-alt{
  margin-right:5px;
}
</style>
