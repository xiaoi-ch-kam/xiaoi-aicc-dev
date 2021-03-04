<template>
  <div>
    <el-row>
      <el-col :span="24" class="kbs-widgets-tags">
        <el-form :model="custInfo" label-position="left" label-width="110px" size="small">
          <el-form-item label="来访次数" class="kbs-short-input">
            <el-input type="number" v-model="custInfo.visitNum">
            </el-input>
          </el-form-item>
          <el-form-item label="用户昵称" class="kbs-short-input">
            <el-input type="text" v-model="custInfo.userNickname">
            </el-input>
          </el-form-item>
          <el-form-item label="用户姓名" class="kbs-short-input">
            <el-input type="text" v-model="custInfo.userName">
            </el-input>
          </el-form-item>
          <el-form-item label="企业名称" class="kbs-short-input">
            <el-input type="text" v-model="custInfo.compName">
            </el-input>
          </el-form-item>
          <el-form-item label="企业地址" class="kbs-short-input">
            <el-input type="text" v-model="custInfo.compAddress">
            </el-input>
          </el-form-item>
          <el-form-item label="性别" class="kbs-short-input">
            <el-select clearable v-model="custInfo.gender">
              <el-option label="男" value="男" />
              <el-option label="女" value="女" />
            </el-select>
          </el-form-item>
          <el-form-item label="年龄" class="kbs-short-input">
            <el-input type="number" v-model="custInfo.custAge">
            </el-input>
          </el-form-item>
          <el-form-item label="英文名" class="kbs-short-input">
            <el-input type="text" v-model="custInfo.userEngName">
            </el-input>
          </el-form-item>
          <el-form-item label="联系电话" class="kbs-short-input">
            <el-input type="text" v-model="custInfo.mobilePhone">
            </el-input>
          </el-form-item>
          <el-form-item label="用户级别" class="kbs-short-input">
            <el-select clearable v-model="custInfo.custLevel">
              <el-option label="默认" value="默认" />
              <el-option label="VIP" value="VIP" />
              <el-option label="普通" value="普通" />
            </el-select>
          </el-form-item>
          <el-form-item label="职务" class="kbs-short-input">
            <el-input type="text" v-model="custInfo.position">
            </el-input>
          </el-form-item>
          <el-form-item label="部门" class="kbs-short-input">
            <el-input type="text" v-model="custInfo.dept">
            </el-input>
          </el-form-item>
          <el-form-item label="备注" class="kbs-short-input">
            <el-input type="text" v-model="custInfo.remark">
            </el-input>
          </el-form-item>
          <el-form-item label="" class="kbs-short-input">
            <el-button type="primary" size="medium" style="margin-top: 5px" @click="saveInfo">提交保存</el-button>
          </el-form-item>
        </el-form>
      </el-col>
    </el-row>
  </div>
</template>

<script>
export default {
  name: 'UserTest',
  data() {
    return {
      custInfo: {
        visitNum: 0,
        userNickname: '这是一个用户昵称',
        userName: '天凉神破',
        compName: '企业名称',
        compAddress: '火星霸总国王者大道666号天下第一公司',
        gender: '女',
        custAge: 18,
        userEngName: 'King',
        mobilePhone: '18866669999',
        custLevel: '普通',
        position: '总裁',
        dept: '领导部',
        remark: '霸气十足'
      }
    }
  },
  methods: {
    saveInfo() {
      alert('提交保存')
    }
  }
}
</script>
<style lang="sass">
.kbs-widgets-tags
  padding: 0 18px !important
  margin-top: 10px

.kbs-short-input .el-input
  width: 232px

.kbs-short-input .el-select
  width: 232px

.el-table tbody tr:hover > td
  background-color: #fafafa !important

input::-webkit-outer-spin-button,
input::-webkit-inner-spin-button
  -webkit-appearance: none

input[type="number"]
  -moz-appearance: textfield
</style>
