<script setup>
import { ref } from 'vue'

// 순수 javascript 영역으로 생각하면 편하다.
// 컴포넌트 생명주기인 setup이 실행되는 자리, setup은 마운트 되기 이전 초기 단계이다.

// ref쪽이 훅과 동일한 영역
const count = ref(0)
</script>

<template>
  <!-- div 루트 엘리먼트 없어도 가능 -->
  <div>
    <button @click="count++">클릭 횟수 : {{ count }}</button>
  </div>
</template>
