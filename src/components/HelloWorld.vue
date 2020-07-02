<template>
  <div>
    <div id="reply"></div>
  </div>
</template>

<script lang="ts">
  import { Vue, Component, Prop, Watch } from 'vue-property-decorator';


  @Component({})
  export default class HelloWorld extends Vue {
    @Prop({ required: true, default: {} })
    private data: any;

    @Watch('data', { deep: true })
    initData() {
      this.getOption();
    }

    getOption() {

    }
  }
</script>
<style lang="scss" scoped>
  #reply {
    height: 500px;
  }
</style>
