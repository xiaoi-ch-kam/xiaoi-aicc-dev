<template>
  <el-row>
    <el-col :span="24">
      <el-table :data="tableData">
        <el-table-column prop="month" label="月份" width="80px" align="center">
        </el-table-column>
        <el-table-column prop="sum" label="接待总数" align="center">
        </el-table-column>
        <el-table-column prop="avg" label="平均接待时长（分钟）" align="center">
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
          month: '2021-02',
          sum: 347,
          avg: 18
        }, {
          month: '2021-01',
          sum: 380,
          avg: 21
        }, {
          month: '2020-12',
          sum: 476,
          avg: 23
        }, {
          month: '2020-11',
          sum: 511,
          avg: 12
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
