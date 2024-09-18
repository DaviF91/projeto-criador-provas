<template>
    <span
      :style="{ width: computedWidth, height: computedHeight }"
       class="inline-flex items-center justify-center rounded-md bg-green-50 px-2 py-1 text-xs font-medium text-green-700 ring-1 ring-inset ring-green-600/20 cursor-pointer"
    >
      <slot>Badge</slot> 
    </span>
  </template>
  
  <script>
  export default {
    name: 'ButtonAdd',
    props: {
      width: {
        type: String,
        default: 'auto'
      },
      height: {
        type: String,
        default: 'auto'
      }
    },
    computed: {
      computedWidth() {
        return this.width;
      },
      computedHeight() {
        return this.height;
      }
    }
  }
  </script>