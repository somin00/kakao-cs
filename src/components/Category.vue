<template>
    <ul class="category-list">
      <li class="category-item" v-for="(categoryName, i) in categoryNameList" :key="i">
        <a>{{categoryName}}</a>
      </li>
    </ul>
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
.category-list{
  list-style:none;
  padding:0px;
  width:160px;
}

.category-item{
  margin-bottom:20px;
  font-size:14px;
}

.category-item:first-child{
  text-decoration:underline;
  font-weight:bold;
}

.category-item:hover{
  text-decoration: underline;
  font-weight:bold;
}
</style>
