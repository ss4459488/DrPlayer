<template>
  <!-- 内容上方面包屑-->
  <a-breadcrumb :style="{ margin: '16px 0' }">
    <a-breadcrumb-item>Home</a-breadcrumb-item>

    <div class="header-left">
      <a-button shape="circle" @click="goBack">
        <template #icon>
          <icon-left/>
        </template>
      </a-button>
      <a-button shape="circle" @click="goForward">
        <template #icon>
          <icon-right/>
        </template>
      </a-button>
      <a-button shape="circle" @click="refreshPage">
        <template #icon>
          <icon-refresh/>
        </template>
      </a-button>
    </div>

    <!-- 中间搜索框 -->
    <div class="header-center">
      <a-input-search
          placeholder="请输入搜索内容"
          enter-button
          @search="onSearch"
          style="width: 300px;"
      />
    </div>

    <!-- 右侧控制按钮 -->
    <div class="header-right">
      <a-button shape="circle" @click="minimize">
        <template #icon>
          <icon-shrink/>
        </template>
      </a-button>
      <a-button shape="circle" @click="maximize">
        <template #icon>
          <icon-expand/>
        </template>
      </a-button>
      <a-button shape="circle" @click="closeWindow">
        <template #icon>
          <icon-close/>
        </template>
      </a-button>

    </div>

  </a-breadcrumb>

  <!-- 内容区域 -->
  <a-layout-content class="content">
    <div>
      <h1>主页</h1>
      <p>这是主页页面的内容。</p>
    </div>
  </a-layout-content>

</template>

<script setup>
const goBack = () => {

}
const goForward = () => {

}
const refreshPage = () => {

}
const onSearch = () => {

}
const minimize = () => {

}
const maximize = () => {

}
const closeWindow = () => {

}
</script>

<style scoped>
/* 页面样式 */

.header-left,
.header-right {
  display: flex;
  align-items: center;
}

.header-left button,
.header-right button {
  margin-right: 10px;
}

.header-center {
  flex-grow: 1;
  display: flex;
  justify-content: center;
}

.header-center a-input-search {
  width: 300px;
}
</style>