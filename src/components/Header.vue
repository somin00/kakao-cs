<template>
 <header>
   <div class="setting">
     <button class="lang-button">한국어</button>
     <img src="https://www.mommyestimate.com/img/arrow_down_black.png" alt="언어보기" class="more-lang">
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
  margin:10px auto 20px;
  justify-content: flex-end;
}

.lang-button{
  border:none;
  background-color: #fff;
  font-size: 12px;
}

.more-lang{
  width:7px;
  height:7px;
  margin:6px 5px 0px 0px;
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
