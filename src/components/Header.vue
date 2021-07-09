<template>
 <header>
   <div class="setting">
     <button class="lang-button">한국어</button>
     <a href="" class="login-link">로그인</a>
   </div>
   <div class="head">
     <img src="../assets/cslogo.gif" alt="kakao 고객센터" class="cslogo">
     <Search/>
   </div>
 </header>
</template>

<script>
import Search from './Search.vue';

export default {
  name: 'Header',
  components: {
    Search,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
header{
  display:flex;
  flex-direction: column;
  border-bottom:1px solid #e8e8e8;
}

.setting{
  width:990px;
  display:flex;
  margin:0px auto 20px;
  justify-content: flex-end;
}

.lang-button{
  border:none;
  background-color: #fff;
  font-size: 12px;
}

.login-link{
  text-decoration: none;
  color:black;
  font-size:13px;
}

.head{
  display:flex;
  width:990px;
  margin:10px auto 40px;
}

.cslogo{
  width:200px;
  height:35px;
  margin-top:5px;
}

</style>
