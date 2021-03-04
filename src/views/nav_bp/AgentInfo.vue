<template>
  <el-row>
    <el-col :span="24">
      <el-table :data="tableData" class="bp_table">
        <el-table-column prop="id" label="坐席编号" width="150px">
        </el-table-column>
        <el-table-column prop="name" label="坐席名称" width="80px">
        </el-table-column>
        <el-table-column prop="sex" label="性别">
        </el-table-column>
        <el-table-column prop="address" label="地区">
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
          sex: '男',
          address: '深圳'
        }, {
          id: '012311458035',
          name: '李四',
          sex: '女',
          address: '深圳'
        }, {
          id: '598311234367',
          name: '王五',
          sex: '女',
          address: '广州'
        }
      ]
    }
  }
}
</script>

<style  lang="scss" scoped>
.bp_table {
  margin: 10px 20px;
}
</style>
