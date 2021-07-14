<template>
  <main>
    <Path :home="home" :serviceName="serviceName" :selectedCategoryName="selectedCategoryName"/>
    <div class="main">
     <div class="service">
      <h2>카카오톡 지갑</h2>
      <Category :categoryNameList="categoryNameList"
      :changeCategory="changeCategory" :selectedCategoryName="selectedCategoryName"/>
     </div>
     <Contents :selectedQuestionList="selectedQuestionList"
     :categoryNameList="categoryNameList" :selectedCategoryName="selectedCategoryName"/>
    </div>
  </main>
</template>
<script>
import Category from './Category.vue';
import Contents from './Contents.vue';
import Path from './Path.vue';
import data from '../data/data';

export default {
  name: 'Main',
  components: {
    Category,
    Contents,
    Path,
  },
  data() {
    return {
      categoryNameList: ['일반', '인증서', '서비스 이용', 'MY 비밀번호', '디지털 ID', '지갑 QR'],
      selectedQuestionList: data['일반'],
      home: '홈',
      serviceName: '카카오톡 지갑',
      selectedCategoryName: '일반',
    };
  },
  methods: {
    changeCategory(categoryName) {
      this.selectedCategoryName = categoryName;
      this.selectedQuestionList = data[categoryName];
    },
  },
};
</script>
<style>
main>.main{
  width:990px;
  margin:auto;
  display:flex;
  justify-content: center;
}
.service{
  width:180px;
}

h2{
  width:160px;
  font-size:20px;
  margin:40px 0px;
}

</style>
