<template>
  <div class="sp-event-dropdown">
    <select v-model="events">
      <option v-for="event in events"
        :value="event.symbol"
        :selected="event == selected ? 'selected' : ''"
        :key="event.symbol">
        {{event.title}}
      </option>
    </select>
  </div>
</template>

<script>

export default {
  name: 'EventDropdown',
  data () {
    return {
      events: [
        { symbol: 'wicked', title: 'Wicked' },
        { symbol: 'mamma-mia', title: 'Mamma Mia!' },
        { symbol: '42nd-Street', title: '42nd Street' },
        { symbol: 'jamie', title: 'Everybodys talking about Jamie' },
        { symbol: 'the-book-of-mormon', title: 'The Book of Mormon' }
      ],
      selected: 'wicked'
    }
  }
}
</script>

<style scoped lang="scss">

.sp-event-dropdown {
  dispaly: flex;
  flex: 1 1 auto;
  padding: 5px;
  background: white;
  color: black;
}

</style>
