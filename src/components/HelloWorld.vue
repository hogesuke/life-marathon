<template>
  <div>
    {{ state.old }}
  </div>
</template>

<script lang="ts">
import { createComponent, reactive, ref } from '@vue/composition-api'

export default createComponent({
  name: 'LifeMarathon',
  props: {
    msg: String,
  },
  setup() {
    const state = reactive({
        old: 30
    })

    return {
      state
    }
  }
})
</script>

<style scoped>
</style>
