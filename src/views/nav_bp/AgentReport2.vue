<template>
  <el-row>
    <el-col :span="24">
      <el-table :data="tableData">
        <el-table-column prop="id" label="坐席编号" width="150px">
        </el-table-column>
        <el-table-column prop="name" label="坐席" width="80px">
        </el-table-column>
        <el-table-column prop="count_sum" label="本月接待人数">
        </el-table-column>
        <el-table-column prop="count_today" label="当日接待人数">
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
          id: '012311231231',
          name: '张三',
          count_sum: 89,
          count_today: 7
        }, {
          id: '012311458035',
          name: '李四',
          count_sum: 57,
          count_today: 5
        }, {
          id: '598311234367',
          name: '王五',
          count_sum: 77,
          count_today: 8
        }
      ]
    }
  }
}
</script>
