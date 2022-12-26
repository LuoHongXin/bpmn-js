<script setup lang="ts">
// 引入相关的依赖
import BpmnModeler from "bpmn-js/lib/Modeler";
import { ref, onMounted } from "vue";
const canvas = ref();
// 初始化
const init = () => {
  console.log(canvas.value, "canvas");
  // 获取到属性ref为“canvas”的dom节点
  // 建模
  // const bpmnModeler = ref(
  //   new BpmnModeler({
  //     container: canvas,
  //   })
  // );
  // return { bpmnModeler };
};

onMounted(() => {
  init();
});
</script>

<template>
  <div ref="canvas"></div>
</template>

<style scoped></style>
