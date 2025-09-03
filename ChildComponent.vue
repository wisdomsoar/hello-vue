<template>
  <div>
    <input
      type="text"
      :value="message"
      @input="$emit('update:message', $event.target.value)"
    />
  </div>
</template>

<script>
export default {
  props: ['message']
}
</script>