<script setup lang="ts">
import logo from '../../assets/logo.svg'
import { ref } from 'vue'

const input = ref('')
</script>

<template>
  <div class="Home">
    <div class="fuzhou">福州</div>
    <div class="english">Smart Library</div>
    <div class="chinese">智慧图书馆</div>
    <div class="logo">
      <img :src="logo" alt="logo" id="logo" />
    </div>
    <div class="search">
      <el-input
        v-model="input"
        placeholder="输入书名后回车以搜索"
        size="large"
      />
    </div>
  </div>
</template>

<style>
.Home {
  height: calc(100vh - 64px);
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
  display: flex;
  background-image: url('../../assets/cover.svg');
}
.fuzhou {
  background-color: #7787a2;
  color: #fff;
  text-align: center;
  border-radius: 8px;
  top: 120px;
  left: 100px;
  font-size: 24px;
  position: absolute;
  width: 80px;
  height: 40px;
  display: flex;
  flex-direction: column;
  justify-content: center;
}
.english {
  position: absolute;
  margin: calc(170px - 64px) 0px 0px 100px;
  font-size: 92px;
  font-weight: 700;
  color: #2c3645;
}
.chinese {
  position: absolute;
  font-size: 92px;
  color: #2c3645;
  font-weight: 900;
  margin: calc(260px - 64px) 0px 0px 100px;
}
.logo {
  position: absolute;
  margin: calc(410px - 64px) 0px 0px 100px;
  width: 80px;
  height: 80px;
  padding: 20px;
  background-color: rgba(255, 255, 255, 0.8);
  border-radius: 24px;
  backdrop-filter: blur(10px);
}
.search {
  position: absolute;
  top: 600px;
  left: 300px;
  right: 300px;
}
</style>
