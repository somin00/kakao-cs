<template>
 <div class="navigation">
   <div class="path">
     <ul>
       <li><a href="" class="path-link">홈</a></li>
       <li>
         <span>></span>
         <a href="" class="path-link">카카오톡 지갑</a>
       </li>
       <li>
         <span>></span>
         <a href="" class="path-link" v-for="path in pathNameList" :key="path">{{path}}</a>
       </li>
     </ul>
   </div>
 </div>
</template>
<script>
export default {
  name: 'Path',
  data() {
    return {
      pathNameList: ['일반'],
    };
  },
};
</script>
<style>

.navigation{
  border-bottom:1px solid #e8e8e8;
}
.path{
  width:990px;
  margin:auto;
  font-size:14px;
}

.path>ul{
  margin-left:-35px;
  list-style:none;
  display:flex;
}

.path-link{
  text-decoration: none;
  color:black;
}
</style>
