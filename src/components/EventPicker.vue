<template>
  <div class="sp-event-picker">
    Pick me
  </div>
</template>

<script>
export default {
  name: 'EventPicker',
  props: {
    msg: String
  }
}
</script>

<style scoped lang="scss">

.sp-event-picker {
  dispaly: flex;
  flex: 1 1 auto;
  padding: 5px;
  background: #0576ae;
  color: white;
}

</style>
