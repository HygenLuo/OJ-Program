<template>
  <div id="#app">
    <BasicLayout />
  </div>
  <nav>
    <router-link to="/">Home</router-link>
    |
    <router-link to="/about">About</router-link>
  </nav>
</template>

<style>
#app {
}
</style>
<script setup lang="ts">
import BasicLayout from "@/layouts/BasicLayout.vue";
import { onMounted } from "vue";

/**
 * 全局初始化函数， 有全局单次调用的代码都可以写到这里
 */

const doInit = () => {
  console.log("Welcome!");
};

onMounted(() => {
  doInit();
});
</script>
