<template>
  <el-row>
    <el-col :span="24">
      <el-table :data="tableData">
        <el-table-column prop="id" label="坐席编号" width="150px">
        </el-table-column>
        <el-table-column prop="name" label="坐席" width="80px">
        </el-table-column>
        <el-table-column prop="count_sum1" label="发出评价数">
        </el-table-column>
        <el-table-column prop="count_sum2" label="收到评价数">
        </el-table-column>
        <el-table-column prop="count1" label="非常满意">
        </el-table-column>
        <el-table-column prop="count2" label="满意">
        </el-table-column>
        <el-table-column prop="count3" label="一般">
        </el-table-column>
        <el-table-column prop="count4" label="不满意">
        </el-table-column>
        <el-table-column prop="count5" label="非常不满意">
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
          count_sum1: 33,
          count_sum2: 29,
          count1: 18,
          count2: 7,
          count3: 3,
          count4: 0,
          count5: 1
        }, {
          id: '012311458035',
          name: '李四',
          count_sum1: 40,
          count_sum2: 35,
          count1: 20,
          count2: 7,
          count3: 5,
          count4: 3,
          count5: 0
        }, {
          id: '598311234367',
          name: '王五',
          count_sum1: 39,
          count_sum2: 38,
          count1: 20,
          count2: 8,
          count3: 9,
          count4: 0,
          count5: 1
        }
      ]
    }
  }
}
</script>
