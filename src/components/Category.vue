<template>
    <ul class="category-list">
      <li class="category-item"
      v-for="(categoryName, i) in categoryNameList" :key="i"
      @click="changeCategory(categoryName)">
        <a :class="{'bold-underline': categoryName==selectedCategoryName}">{{categoryName}}</a>
      </li>
    </ul>
</template>
<script>
export default {
  name: 'Category',
  props: ['categoryNameList', 'changeCategory', 'selectedCategoryName'],
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

.category-item:hover{
  text-decoration: underline;
  font-weight:bold;
}

.bold-underline{
  text-decoration: underline;
  font-weight: bold;
}

</style>
