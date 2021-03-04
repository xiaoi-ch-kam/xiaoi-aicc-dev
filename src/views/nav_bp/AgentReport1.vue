<template>
  <el-row>
    <el-col :span="24">
      <el-table :data="tableData">
        <el-table-column prop="id" label="坐席编号" width="150px">
        </el-table-column>
        <el-table-column prop="name" label="坐席" width="80px">
        </el-table-column>
        <el-table-column prop="start_time" label="上线时刻">
        </el-table-column>
        <el-table-column prop="end_time" label="下线时刻">
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
          start_time: '2021-02-28 08:43:34',
          end_time: '2021-02-28 19:20:33'
        }, {
          id: '012311458035',
          name: '李四',
          start_time: '2021-02-28 09:10:20',
          end_time: '2021-02-28 18:22:46'
        }, {
          id: '598311234367',
          name: '王五',
          start_time: '2021-02-28 08:58:02',
          end_time: '2021-02-28 18:03:18'
        }
      ]
    }
  }
}
</script>
