<template>
  <div class="about">
    <h1>This is an about page</h1>
    <el-button>el-button</el-button>
    <div>
      <el-radio v-model="radio" label="1">备选项11</el-radio>
      <el-radio v-model="radio" label="2">备选项22</el-radio>
    </div>
  </div>
</template>
<script>
export default {
  name: 'about',
  data () {
    return {
      radio: '1'
    }
  }
}
</script>

<style>
</style>
