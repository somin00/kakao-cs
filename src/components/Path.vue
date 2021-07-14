<template>
 <div class="navigation">
   <div class="path">
     <ul>
       <li><a href="" class="path-link">{{home}}</a></li>
       <li>
         <span>></span>
         <a href="" class="path-link">{{serviceName}}</a>
       </li>
       <li>
         <span>></span>
         <a href="" class="path-link">{{selectedCategoryName}}</a>
       </li>
     </ul>
   </div>
 </div>
</template>
<script>
export default {
  name: 'Path',
  props: ['home', 'serviceName', 'selectedCategoryName'],
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

.path-link:not(:first-child){
  margin-left:10px;
}

.path-link:hover{
  text-decoration:underline;
}

ul>li{
  margin-right:10px;
}
</style>
