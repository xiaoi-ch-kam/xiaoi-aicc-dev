<template>
  <el-row>
    <el-col :span="24">
      <el-table :data="tableData">
        <el-table-column prop="date" label="日期" width="80px" align="center">
        </el-table-column>
        <el-table-column prop="start_time" label="上线时刻" align="center">
        </el-table-column>
        <el-table-column prop="end_time" label="下线时刻" align="center">
        </el-table-column>
      </el-table>
    </el-col>
  </el-row>
</template>

<script>
export default {
  data() {
    return {
      tableData: [
        {
          date: '2021-02-28',
          start_time: '08:30:23',
          end_time: '19:23:45'
        }, {
          date: '2021-02-27',
          start_time: '09:34:36',
          end_time: '19:48:50'
        }, {
          date: '2021-02-26',
          start_time: '08:52:15',
          end_time: '18:15:54'
        }, {
          date: '2021-02-25',
          start_time: '08:48:29',
          end_time: '18:45:31'
        }
      ]
    }
  },
  methods: {
  }
}
</script>
<style lang="sass" scoped>
</style>
