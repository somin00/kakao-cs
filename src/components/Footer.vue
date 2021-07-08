<template>
 <footer>
   <div class="list">
     <div class="additional-list">회사소개</div>
     <div class="additional-list">이용약관</div>
     <div class="additional-list personal-info">개인정보처리방침</div>
     <div class="additional-list">운영정책</div>
     <div class="additional-list">청소년보호정책</div>
     <div class="additional-list">권리침해신고안내</div>
     <div class="additional-list">공지사항</div>
   </div>
   <div class="bottom">
     <div class="copyright">Copyright © Kakao Corp. All rights reserved.</div>
   </div>
 </footer>
</template>

<script>
export default {
  name: 'Footer',
};
</script>

<style>
footer{
  border-top:1px solid black;
}

footer>div{
    width:990px;
    margin:auto;
}
.list{
  display:flex;
  margin-top:10px;
}

.list>.additional-list{
  font-size:13px;
  margin-right:10px;
}

.personal-info{
  font-weight: bold;
}

.bottom{
  display:flex;
  margin-top:2px;
}

.copyright{
  font-size:12px;
  margin-top:10px;
}
.kakaotalk{
  margin-left:auto;
}
</style>
