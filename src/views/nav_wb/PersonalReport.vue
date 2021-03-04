<template>
  <div style="height: 100%;">
    <Menu :routeData="routeData"></Menu>
  </div>
</template>

<script>
import Menu from '../components/Menu'

export default {
  components: { Menu },
  data() {
    return {
      routeData: [
        {
          name: '个人上线统计',
          path: '/personalReport/personalReport1'
        },
        {
          name: '个人接待',
          path: '/personalReport/reportGroup1',
          children: [
            {
              name: '个人接待统计',
              path: '/personalReport/reportGroup1/personalReport2'
            },
            {
              name: '个人评价分析',
              path: '/personalReport/reportGroup1/personalReport3'
            }
          ]
        }
      ]
    }
  }
}
</script>
