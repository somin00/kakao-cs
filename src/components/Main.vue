<template>
  <main>
    <Path/>
    <div class="main">
     <div class="service">
      <h2>카카오톡 지갑</h2>
      <Category/>
     </div>
     <Contents/>
    </div>
  </main>
</template>
<script>
import Category from './Category.vue';
import Contents from './Contents.vue';
import Path from './Path.vue';

export default {
  name: 'Main',
  components: {
    Category,
    Contents,
    Path,
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
