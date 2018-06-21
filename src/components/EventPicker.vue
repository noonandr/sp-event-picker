<template>
  <div class="sp-event-picker">
    <EventDropdown/>
  </div>
</template>

<script>

import EventDropdown from '@/components/EventDropdown.vue'

export default {
  name: 'EventPicker',
  components: {
    EventDropdown
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
