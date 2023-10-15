<template>
  <div
    class="bg-[url('./assets/imgs/bg.jpg')] bg-cover bg-center h-screen text-white p-5 flex overflow-hidden"
  >
    <!-- 左 -->
    <div class="flex flex-col flex-1 p-3 mr-5 bg-opacity-50 bg-slate-800">
      <!-- 横向柱状图 -->
      <HorizontalBar class="box-border h-1/3 pd-4" />
      <!-- 雷达图 -->
      <RadarBar class="box-border h-1/3 pd-4" />
      <!-- 关系图 -->
      <Relation class="h-1/3" />
    </div>
    <!-- 中 -->
    <div class="flex flex-col w-1/2 mr-5">
      <!-- 数据总览图 -->
      <TotalData class="p-3 bg-opacity-50 bg-slate-800" />
      <!-- 地图可视化 -->
      <MapChart class="flex-1 p-3 mt-4 bg-opacity-50 bg-slate-800" />
    </div>
    <!-- 右 -->
    <div class="flex flex-col flex-1 p-3 bg-opacity-50 bg-slate-800">
      <!-- 竖向柱状图 -->
      <VerticalBar class="box-border h-1/3 pd-4" />
      <!-- 环形图 -->
      <RingBar class="box-border h-1/3 pd-4" />
      <!-- 文档云图 -->
      <WordCloud class="h-1/3" />
    </div>
  </div>
</template>

<script setup>
import HorizontalBar from "@/components/HorizontalBar.vue";
import MapChart from "@/components/MapChart.vue";
import RadarBar from "@/components/RadarBar.vue";
import Relation from "@/components/Relation.vue";
import RingBar from "@/components/RingBar.vue";
import TotalData from "@/components/TotalData.vue";
import VerticalBar from "@/components/VerticalBar.vue";
import WordCloud from "@/components/WordCloud.vue";
</script>

<style lang="scss" scoped></style>
