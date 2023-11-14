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
  let buttonClass;

  switch (props.variant) {
    case 'primary':
      buttonClass = 'mt-8 text-lg sm:text-xl bg-gray-800 p-4 rounded transition-colors hover:bg-white hover:text-gray-800 font-semibold';
      break;
    case 'secondary':
      buttonClass = 'text-m bg-white border-blue-500 text-blue-600 p-2 hover:bg-blue-500 hover:text-white rounded font-semibold';
      break;
    case 'tertiary':
      buttonClass = 'text-m bg-gray-600 text-gray-200 p-2 hover:bg-blue-500 hover:text-white rounded font-semibold';
      break;
    default:
      buttonClass = 'text-m bg-white border-blue-500 text-blue-600 p-2 hover:bg-blue-500 hover:text-white rounded font-semibold';
      break;
  }

  return buttonClass;
};
</script>
