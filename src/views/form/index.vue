<template>
  <div width="100%" height="100%">
    <iframe :src="url" />
  </div>
</template>

<script>
export default {
  data() {
    return {
      url: 'http://10.30.50.121:1234/dataquery/index'
    }
  },
  methods: {
    onSubmit() {
      this.$message('submit!')
    },
    onCancel() {
      this.$message({
        message: 'cancel!',
        type: 'warning'
      })
    }
  }
}
</script>

<style scoped>
.line{
  text-align: center;
}
</style>

