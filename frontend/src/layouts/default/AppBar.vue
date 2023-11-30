<template>
  <v-app-bar flat>
    <v-app-bar-title class="appbar"
      ><span class="appbarfont">로그인</span
      ><span class="appbarfont">회원가입</span>
      <span class="appbarfont">고객센터</span></v-app-bar-title
    >
  </v-app-bar>
</template>

<script setup>
//
</script>
<style>
.appbar {
  position: absolute;
  right: 10px;
}
.appbarfont {
  font-size: 14px;
  margin-right: 16px;
}
.appbar span {
  cursor: pointer;
}
</style>
