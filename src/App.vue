<template>
<el-container>
  <el-header>
    <el-menu
    :default-active="activeIndex"
    mode="horizontal"
    class="menu"
    background-color="#4B4B4B59"
    text-color="#fff"
    active-text-color="#FFF">
    <el-menu-item index="1">PiPimage</el-menu-item>
    <el-menu-item index="2"><a href="">首页</a></el-menu-item>
    <el-menu-item index="3"><a href="">生鲜图片下载</a></el-menu-item>
    <el-menu-item index="4"><a href="">API接口</a></el-menu-item>
    <el-menu-item index="5"><a href="">品牌商入驻</a></el-menu-item>
    <el-menu-item index="6"><a href="">我的订单</a></el-menu-item>
    <el-menu-item index="7"><a href="">我的购物车</a></el-menu-item>
    <el-menu-item index="8"><a href="">ADMIN</a></el-menu-item>
  </el-menu>
  </el-header>
    <el-main class="main">
      <div>
    <p>
      <span>PiPimage</span>
      超市便利店图片覆盖超80%，即刻登录下载
    </p>
    <el-input
      placeholder="请输入内容"
      v-model="input3"
      class="input-with-select"
    >
      <template #prepend>
        <el-select v-model="select" placeholder="请选择">
          <el-option label="条形码搜索" value="1"></el-option>
          <el-option label="关键词搜索" value="2"></el-option>
          <el-option label="条形码上传" value="3"></el-option>
        </el-select>
      </template>
      <template #append>
        <el-button icon="el-icon-search"></el-button>
      </template>
    </el-input>
  </div>
  <div>图片展示</div>
  <div>
    购买方式
    <div></div>
  </div>
    </el-main>
    <el-footer>
      <el-row>
        <el-col :span="2" :offset="2">PiPimage</el-col>
  <el-col :span="14">
    <ul>
      <li>商务合作：idones@163.com</li>
      <li>联系我们：13011051863</li>
      <li>图片无法下载联系：idones@163.com</li>
    </ul>
  </el-col>
  <el-col :span="4">
    <ul>
      <li>生鲜图片下载</li>
      <li>常见问题</li>
      <li>API接口</li>
      <li>问题反馈</li>
    </ul>
  </el-col>
      </el-row>
      <div class="line"></div>
      <p>© PiPimage 浙ICP备2021005116号-1 杭州银灰色信息技术有限公司</p>
    </el-footer>
  </el-container>
</template>

<script lang="ts">
import { defineComponent, ref } from 'vue'

export default defineComponent({
  name: 'App',
  components: {
    
  },
  data() {
    return {
    }
  },
  setup() {
    return {
      input1: ref(''),
      input2: ref(''),
      input3: ref(''),
      select: ref('')
    }
  }
})
</script>

<style>
.el-select .el-input {
  width: 130px;
}
.menu a {
  text-decoration: none;
}
.main {
  background-image: url('./assets/background.png');
  height: 464px;
  width: 100%;
}
</style>