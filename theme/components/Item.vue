<script>
export default {
  props: {
    text: {
      type: String,
      required: true,
      default: '@username'
    },
  },
}
</script>

<template>
  <div class="flex justify-center items-center ml-4">
    <span class="flex justify-center item-center mr-1.5">
      <slot />
    </span>
    <span class="ml-1">
      {{text}}
    </span>
  </div>
</template>
