<template>
  <!-- 采用左右布局 -->
  <el-container class="ht100">

    <!-- 左侧侧边栏 -->
    <el-aside :style="subNavDynamicStyle">
      <!-- <div>Menu</div> -->
      <el-menu background-color="#f7f8fa" style="border-right: none;" router :default-active="$route.path">
        <div v-for="(r)  in routeData" :key="r.path">
          <el-submenu v-if="r.children" :index="'/dev' + r.path">
            <template slot="title">
              <span>{{ r.name }}</span>
            </template>
            <el-menu-item :index="'/dev' + child.path" v-for="(child)  in r.children" :key="'/dev' + child.path">
              {{ child.name }}
            </el-menu-item>
          </el-submenu>
          <el-menu-item :index="'/dev' + r.path" v-else>
            <span slot="title">{{ r.name }}</span>
          </el-menu-item>
        </div>
      </el-menu>
    </el-aside>

    <!-- 右侧主体面板:通过动态路由加载 -->
    <el-main>
      <router-view></router-view>
    </el-main>

  </el-container>
</template>

<script>
export default {
  data() {
    return {
      subNavDynamicStyle: {
        width: '180px',
        // height: '100%',
        display: 'block',
        background: '#f7f8fa',
        'border-right': '1px solid #e1e3e6'
      }
    }
  },
  props: {
    routeData: {
      type: Array,
      default: () => {
        return []
      }
    }
  }
}
</script>
