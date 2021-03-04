<template>
  <el-row>
    <el-col :span="24">
      <el-table :data="tableData">
        <el-table-column prop="month" label="月份" width="80px" align="center">
        </el-table-column>
        <el-table-column prop="count_sum1" label="发出评价数" align="center">
        </el-table-column>
        <el-table-column prop="count_sum2" label="收到评价数" align="center">
        </el-table-column>
        <el-table-column prop="count1" label="非常满意" align="center">
        </el-table-column>
        <el-table-column prop="count2" label="满意" align="center">
        </el-table-column>
        <el-table-column prop="count3" label="一般" align="center">
        </el-table-column>
        <el-table-column prop="count4" label="不满意" align="center">
        </el-table-column>
        <el-table-column prop="count5" label="非常不满意" align="center">
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
          count_sum1: 312,
          count_sum2: 296,
          count1: 189,
          count2: 93,
          count3: 6,
          count4: 3,
          count5: 5
        }, {
          month: '2021-01',
          count_sum1: 349,
          count_sum2: 312,
          count1: 154,
          count2: 117,
          count3: 37,
          count4: 3,
          count5: 1
        }, {
          month: '2020-12',
          count_sum1: 423,
          count_sum2: 372,
          count1: 139,
          count2: 158,
          count3: 72,
          count4: 3,
          count5: 0
        }, {
          month: '2020-11',
          sum: 511,
          count_sum1: 489,
          count_sum2: 411,
          count1: 218,
          count2: 117,
          count3: 63,
          count4: 4,
          count5: 9
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
