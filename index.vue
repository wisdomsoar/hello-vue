<template>
  <div>
    <child-component :message="text" @update:message="newVal => text = newVal" />
    <p> MESAGE: {{ text }}</p>
  </div>
</template>

<script>
import ChildComponent from './ChildComponent.vue'

export default {
  components: { ChildComponent },
  data() {
    return {
      text: 'Hello Vue!'
    }
  }
}
</script>