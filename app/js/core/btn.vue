<template>
  <div>
    <div :class="[btnClass,cname]">
      <slot/>
    </div>
  </div>
</template>
<script>
export default {
  props: {
    cname: {
      type: String,
      default: "",
    }
  },
  data() {
    return {
      btnClass: 'btn'
    }
  }
}
</script>

<style lang="scss">
@import "../../css/element.scss"
.btn{
  @inclue btn
}
</style>

