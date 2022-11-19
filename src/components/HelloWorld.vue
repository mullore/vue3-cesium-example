<script setup lang="ts">
import * as Cesium from 'cesium';
import { onMounted } from 'vue';
onMounted(() => {
  const viewer = new Cesium.Viewer('cesiumContainer', {
    infoBox: false, // 禁用沙箱，解决控制台报错
  });
});


</script>

<template>
  <div id="cesiumContainer"></div>
</template>

<style scoped>
#cesiumContainer {
  position: absolute;
  width: 100%;
  height: 100%;
  top: 0px;
  left: 0px;
  margin: 0;
  padding: 0;
  overflow: hidden;
}
</style>
