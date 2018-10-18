<template>
  <div>
    <div :class="['btnClass',cname]">
       <slot></slot>
    </div>
  </div>
</template>
<script>
export default {
  props: {
    cname:{
      type:String,
      default: "",
    }
  },
  data() {
    return {
      btnClass: 'btn'
    }
  },
}
</script>
<style lang="sass">
@import "../../css/element.scss"
.btn {
  @inclue btn
}
</style>

