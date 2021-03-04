<template>
  <div style="height: 100%;" class="icontest">
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
          name: '坐席上线统计',
          path: '/agentReport/agentReport1'
        },
        {
          name: '坐席接待',
          path: '/agentReport/reportGroup1',
          children: [
            {
              name: '接待统计',
              path: '/agentReport/reportGroup1/agentReport2'
            },
            {
              name: '评价分析',
              path: '/agentReport/reportGroup1/agentReport3'
            }
          ]
        }
      ]
    }
  }
}
</script>
