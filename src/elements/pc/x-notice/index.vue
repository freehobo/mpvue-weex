<template>
  <div class="pc-x-notice" element-path="pc/x-notice">
  {{viewModel}}
  </div>
</template>

<script>
  export default {
    name: 'x-notice',
    props: {
      elementData: {}
    },
    data () {
      return {
        viewModel: ''
      }
    },
    mounted () {
      this.init()
    },
    methods: {
      async init () {
        if (this.elementData !== undefined) {
          this.viewModel = this.elementData
        }
      }
    }
  }
</script>

<style lang="less">
  @import '~_style/index.less';
  .pc-x-notice {
  	font-size: @font-size-base;
  }
</style>
