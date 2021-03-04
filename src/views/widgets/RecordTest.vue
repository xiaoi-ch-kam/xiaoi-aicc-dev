<template>
  <el-row>
    <el-col :span="24" class="kbs-widgets-tags">
      <el-table :data="tableData" class="log-table table-main">
        <el-table-column prop="TYPE" label="类别" show-overflow-tooltip minWidth="50px">
        </el-table-column>
        <el-table-column prop="INSURE_START_DATE" label="起始时间">
        </el-table-column>
        <el-table-column prop="INSURE_END_DATE" label="截止时间">
        </el-table-column>
        <el-table-column prop="CITY" label="城市" minWidth="50px">
        </el-table-column>
      </el-table>
    </el-col>
  </el-row>
</template>

<script>
export default {
  name: 'RecordTest',
  data() {
    return {
      tableData: [
        {
          TYPE: '中',
          INSURE_START_DATE: '2020-12-22 00:00:00',
          INSURE_END_DATE: '2020-12-22 23:59:59',
          CITY: '北京'
        }, {
          TYPE: '低',
          INSURE_START_DATE: '2020-12-22 00:00:00',
          INSURE_END_DATE: '2020-12-22 23:59:59',
          CITY: '杭州'
        }
      ]
    }
  }
}
</script>
