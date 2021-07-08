<template>
    <div class="category-list">
      <div v-for="(categoryName, i) in categoryNameList" :key="i">{{categoryName}}</div>
    </div>
</template>
<script>
export default {
  name: 'Category',
  data() {
    return {
      categoryNameList: ['일반', '인증서', '서비스 이용', 'MY 비밀번호', '디지털 ID', '지갑 QR'],
    };
  },
};
</script>
<style>
.category-list>div{
  margin:0px 0px 20px 3px;
  font-size:15px;
}

.category-list{
  margin-top:40px;
}
</style>
