<template>
  <div>
      <input type="text" v-model="test" placeholder=".shop주소 도메인명을 쓰시오."/>
      <buttonL v-on:click="move">이동</buttonL>
  </div>
</template>

<script setup>
import {ref} from 'vue';
const test =ref(' ');

const move = () => {
  location.href='http://'+test.value+'.shop/health';
}



</script>

<style scoped>

</style>