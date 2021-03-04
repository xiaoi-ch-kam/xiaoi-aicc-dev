<template>
  <div class="info">
    <el-row>
      <el-col :span="5"></el-col>
      <el-col :span="10">
        <el-form :model="personalInfo" disabled label-position="left" label-width="110px" size="small">
          <el-form-item label="坐席ID">
            <el-input type="text" v-model="personalInfo.ID">
            </el-input>
          </el-form-item>
          <el-form-item label="坐席昵称">
            <el-input type="text" v-model="personalInfo.nickname">
            </el-input>
          </el-form-item>
          <el-form-item label="坐席姓名">
            <el-input type="text" v-model="personalInfo.userName">
            </el-input>
          </el-form-item>
          <el-form-item label="性别">
            <el-select clearable v-model="personalInfo.gender">
              <el-option label="男" value="男" />
              <el-option label="女" value="女" />
            </el-select>
          </el-form-item>
          <el-form-item label="年龄">
            <el-input type="number" v-model="personalInfo.age">
            </el-input>
          </el-form-item>
          <el-form-item label="所属地区">
            <el-input type="text" v-model="personalInfo.address">
            </el-input>
          </el-form-item>
        </el-form>
      </el-col>
      <el-col :span="9"></el-col>
    </el-row>
  </div>
</template>

<script>
export default {
  data() {
    return {
      personalInfo: {
        ID: '012311231231',
        nickname: '大山',
        userName: '张三',
        gender: '男',
        age: 24,
        address: '深圳'
      }
    }
  },
  methods: {
  }
}
</script>
<style lang="sass" scoped>
.info
  margin: 10px 15px
</style>
