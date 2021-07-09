<template>
    <div class="search-box">
       <input type="text" placeholder="궁금한 점이 있다면 도움말을 검색해 보세요." class="input">
       <button class="submit-button"><i class="fas fa-search"></i></button>
    </div>
</template>
<script>
export default {
  name: 'Search',
};
</script>
<style>
.search-box{
  border:1px solid black;
  width:460px;
  height:46px;
  margin-left:30px;
}

.input{
  border:none;
  width:400px;
  height:44px;
  margin-left:10px;
}

.submit-button{
  border:none;
  background-color: #fff;
}

.fa-search{
  font-size:18px;
}
</style>
