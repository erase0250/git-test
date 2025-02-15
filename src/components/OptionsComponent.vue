// vbase를 입력하여 자동완성 템플릿 이용 // 순서는 상관없으나 공식 홈페이지에서 권장하는 script를
먼저 쓰기

<script>
// script 영역이 작성되는 곳
// data나 생명주기 메소드들을 작성할 수 있다.

export default {
  data() {
    return {
      count: 0,
    }
  },
}
</script>

<template>
  <!-- template : html 작성 영역, 실제로는 JS로 변환됨, vue의 고유 속성을 사용가능! -->
  <div>
    <div class="test">클릭 횟수 : {{ count }}</div>
    <!-- @ 누르면 이벤트 리스너들 자동완성됨 -->
    <button @click="count++">클릭 횟수 : {{ count }}</button>
  </div>
</template>

<style scoped>
/* style scoped */
/* css를 적용 가능한 영역 */
.test {
  color: blue;
}
</style>
