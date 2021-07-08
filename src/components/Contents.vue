<template>
   <div class="category-content">
      <div class="category-name">일반</div>
      <div class="common"><a href="#" class="os">os 공통</a></div>
      <div class="question-list">
        <div class="question-item" v-for="(question, number) in questionList" :key="number">
          <div class="question-number">{{number+1}}</div>
          <a href="#" class="question-string">
            <div class="question">{{question}}</div>
            <div class="detail-button"><i class="fas fa-chevron-down"></i></div>
          </a>
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
export default {
  name: 'Contents',
  data() {
    return {
      questionList: ['카카오 지갑은 어떤 서비스인가요?', '카카오 인증서는 무엇인가요?', '나의 디지털 ID가 무엇인가요?'],
    };
  },
};
</script>
<style>
.category-content{
  width:809px;
  border-left:1px solid black;
  /* margin:15px 0px 60px 58px; */
}

.category-content>div{
  margin-left:58px;
}

.category-name{
  font-size:30px;
  font-weight: bold;
  margin: 20px 0px 30px;
}

.common{
  padding:10px 0px 10px 5px;
  border-top:1px solid black;
}

.os{
  color:black;
  font-weight: bold;
  font-size:16px;
  margin:0px 7px;
}

.question-list{
  padding:20px 0px;
  border-top:1px solid black;
  border-bottom:1px solid black;
}

.question-item{
  display:flex;
  padding:15px 0px;
}

.question-item:not(:last-child){
    border-bottom:1px solid black;
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

.question{
  font-size:14px;
  width:625px;
  margin-right:30px;
}

.detail-button{
  margin-left:auto;
  margin-right:15px;
}

.fa-chevron-down{
  font-size:13px;
}

.inquiry{
  display:flex;
  margin-top:80px;
  padding-bottom:100px;
}

.inquiry-text{
  line-height:46px;
  font-size:13px;
}

.inquiry-button{
  margin-left:auto;
  width:186px;
  height:46px;
}

.fa-pencil-alt{
  margin-right:5px;
}
</style>
