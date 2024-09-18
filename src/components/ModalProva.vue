<template>
    <div v-if="isVisible" class="fixed inset-0 flex items-center justify-center z-50">
      <!-- Sobreposição escura -->
      <div class="fixed inset-0 bg-black opacity-50" @click="close"></div>
  
      <!-- Contêiner do modal com posicionamento relativo -->
      <div class="bg-white p-6 rounded-lg shadow-lg relative z-10">
        <!-- Botão de fechar -->
        <button @click="close" class="absolute top-2 right-2 text-gray-500 hover:text-gray-700">
          <XMarkIcon class="h-6 w-6" />
        </button>
  
        <!-- Conteúdo do modal -->
        <slot></slot>
      </div>
    </div>
  </template>
  
  <script>
  import { XMarkIcon } from '@heroicons/vue/24/outline';
  
  export default {
    name: 'ModalProva',
    components: {
      XMarkIcon
    },
    props: {
      isVisible: {
        type: Boolean,
        default: false
      }
    },
    methods: {
      close() {
        this.$emit('update:isVisible', false);
      }
    }
  }
  </script>
  
  <style scoped>
  /* Adicione estilos adicionais, se necessário */
  </style>
  