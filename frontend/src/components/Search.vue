<template>
  <v-container fluid class="fill-height container">
    <div class="background">
      <div class="search-bar">
        <div>
          <v-img src="@/assets/imgs/vsShop-logo.png" alt="logo" class="logo" />
        </div>
        <div class="field">
          <v-text-field
            clearable
            append-inner-icon="mdi-magnify"
            label=""
            density="compact"
            variant="outlined"
            class="search"
          ></v-text-field>
        </div>
        <div class="mypage">
          <div class="s1">
            <div class="user-icon">
              <v-img
                class="user-icon"
                src="@/assets/imgs/user.png"
                alt="user-icon"
              />
            </div>
            <span>마이페이지</span>
          </div>
          <div class="s2">
            <div class="heart-icon">
              <v-img
                class="heart-icon"
                src="@/assets/imgs/heart.png"
                alt="heart-icon"
              />
            </div>
            <span>찜리스트</span>
          </div>
          <div class="s3">
            <div class="glass-sign">
              <v-img
                class="glass-icon"
                src="@/assets/imgs/glass-sign.png"
                alt="glass-icon"
              />
            </div>
            <span>최근본상품</span>
          </div>
        </div>
      </div>
      <div class="cate-bar">
        <span>전체</span><span>></span><span>생활용품</span><span>></span
        ><span>샴푸</span>
      </div>
      <v-sheet class="category" width="190" elevation="1">
        <p class="title">카테고리</p>
        <p class="sub-title">전체</p>
        <p class="sub-title">생활용품</p>
        <p class="sub-detile">헤어</p>
        <p class="sub-detile">욕실용품</p>
        <p class="sub-detile">수납/정리</p>
        <p class="sub-detile">구강/면도</p>
      </v-sheet>
      <div class="content">
        <div class="sub-title">"검색어"에 대한 검색결과</div>
        <div class="sorting">
          <span
            ><v-img
              class="check-mark"
              width="12"
              src="@/assets/imgs/check-mark.png"
              alt="check-mark"
          /></span>
          <span class="list select">낮은가격순</span>
          <span class="list">높은가격순</span>
          <span class="list">리뷰순</span>
          <span class="list">조회순</span>
        </div>
        <v-sheet elevation="1" class="section">
          <div>
            <v-img
              class="product"
              width="200"
              src="@/assets/imgs/shampoo.png"
              alt="product"
            />
          </div>
          <div class="contents">
            <div class="title">
              <p>부케가르니 니드 샴푸 시그니처</p>
              <p :align="'right'" class="ml">1000ml, 2개</p>
              <p :align="'right'" class="score">
                <span class="s1">4.8</span>/5.0
              </p>
            </div>
            <div class="sub-contents">
              <div class="s1">
                <p>네이버</p>
                <p>최저 판매가</p>
              </div>
              <div class="s2">
                <p :align="'right'" class="discount">
                  50%, <span class="line">44,000</span>
                </p>
                <p :align="'right'" class="price">21,900원</p>
              </div>
            </div>
            <div class="sub-contents-2">무료배송</div>
          </div>
          <div class="link"><span>바로 구매하러 가기</span></div>
        </v-sheet>
      </div>
    </div>
  </v-container>
</template>

<script setup>
//
</script>

<style>
.background {
  margin: 0 auto;
}
.logo {
  width: 180px;
  margin: -21px 15px 0 0;
  cursor: pointer;
}
.search-bar {
  display: flex;
  justify-content: flex-start;
  position: absolute;
  top: 78px;
}
.search-bar .field {
  width: 580px;
  margin-right: 30px;
}
.search-bar .mypage {
  display: flex;
  justify-content: space-between;
  font-size: 12px;
  margin-top: -14px;
}
.search-bar .mypage .s1 {
  margin-right: 18px;
  cursor: pointer;
}
.search-bar .mypage .s2 {
  margin-right: 18px;
  cursor: pointer;
}
.search-bar .mypage .s3 {
  margin-right: 18px;
  cursor: pointer;
}
.search-bar .mypage .s1 .user-icon {
  width: 30px;
  margin-left: 8px;
  margin-bottom: 2px;
}
.search-bar .mypage .s2 .heart-icon {
  width: 35px;
  margin-left: 3px;
  margin-top: 9px;
  margin-bottom: 2px;
}
.search-bar .mypage .s3 .glass-icon {
  width: 32px;
  margin-left: 9px;
  margin-top: 12px;
  margin-bottom: 2px;
}
.search-bar .mypage .s1 {
  display: flex;
  justify-content: center;
  flex-direction: column;
}
.cate-bar {
  position: absolute;
  top: 150px;
  left: 50px;
  padding: 3px 0 0 410px;
  width: 100vw;
  background-color: #f5f5f5;
  height: 30px;
}
.cate-bar > span {
  font-size: 11px;
  margin-right: 8px;
}
.category {
  position: absolute;
  top: 200px;
  font-size: 12px;
  padding: 11px 16px 8px 16px;
}
.category .title {
  font-weight: 600;
  font-size: 13px;
  margin-bottom: 6px;
}
.category .sub-title {
  font-weight: 500;
  font-size: 13px;
  margin-bottom: 6px;
  cursor: pointer;
}
.category .sub-detile {
  font-size: 12px;
  margin: 10px 0 4px 12px;
  cursor: pointer;
}
.content {
  display: flex;
  flex-direction: column;
  height: 415px;
  padding-left: 210px;
}
.sub-title {
  font-weight: 600;
  font-size: 19px;
}
.sorting {
  padding: 4px 0 0 2px;
  margin-bottom: 4px;
}
.sorting span {
  display: inline-block;
  cursor: pointer;
}
.sorting .check-mark {
  margin-right: 2px;
}
.sorting .list {
  font-size: 11px;
  margin-right: 12px;
}
.sorting .select {
  font-weight: 700;
  color: #0a73ae;
}
.section {
  display: flex !important;
  width: 800px;
  height: 220px;
  padding: 10px 0 10px 0;
  cursor: pointer;
}
.contents {
  display: flex;
  flex-direction: column;
  font-size: 16px;
}
.contents .title {
  width: 200px;
  margin-bottom: 16px;
}
.contents .title .score {
  font-size: 14px;
}
.contents .title .s1 {
  color: #14acb6;
}
.contents .sub-contents {
  display: flex;
  margin-top: 12px;
  justify-content: space-between;
}
.contents .sub-contents-2 {
  font-size: 12px;
  margin-top: 12px;
  color: #888888;
  font-weight: 600;
}
.contents .sub-contents .s1 {
  margin-top: 6px;
  font-size: 12px;
  font-weight: 600;
  color: #14acb6;
}
.contents .sub-contents .s2 .discount {
  margin-top: -10px;
  color: #888888;
  font-size: 14px;
}
.contents .sub-contents .s2 .discount .line {
  text-decoration: line-through;
}
.contents .sub-contents .s2 .price {
  font-size: 22px;
  font-weight: 600;
}
.section .link {
  display: flex;
  justify-content: right;
  align-items: center;
  font-size: 20px;
  font-weight: 500;
  width: 400px;
  padding-right: 40px;
}
.section .link span {
  font-size: 25px;
  font-weight: 600;
}
</style>
