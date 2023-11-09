<template>
  <button :class="getClasses()">
    {{ props.text }}
  </button>
</template>

<script setup>
const props = defineProps({
  text: {
    type: String,
    required: true
  },
  variant: {
    type: String,
    default: 'primary'
  }
})
 
const getClasses = () => {
  if (props.variant === 'primary') {
    return 'mt-8 text-lg sm:text-xl bg-gray-800 p-4 rounded transition-colors hover:bg-white hover:text-gray-800 font-semibold';
  } else if (props.variant === 'secondary') {
    return 'text-m bg-white border-blue-500 text-blue-600 p-2 hover:bg-blue-500 hover:text-white rounded font-semibold';
  }

  return '';
}
</script>
