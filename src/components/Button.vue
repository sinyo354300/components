<template>
  <div>
    <button @click="handleClick" ><slot>默认按钮</slot></button>
  </div>
</template>

<script>
  export default {
    props: {
      disabled: {
          type: Boolean,
          default: false,
      }
    },
    methods:{
      handleClick(){
        if(!this.disabled){
          this.$emit("onceClick");
        }
      },
    }
  }
</script>

<style lang="scss" scoped>

</style>