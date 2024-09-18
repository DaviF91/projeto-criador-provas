<template>
    <div>
      <ButtonAdd width="150px" height="150px" @click="showModal">
        <PlusIcon class="h-16 w-16 text-green-500" />
      </ButtonAdd>
      
      <ModalProva v-model:isVisible="isModalVisible">
        
        <h2 class="text-lg font-bold">Formulário</h2>
        <p>Conteúdo do formulário vai aqui.Conteúdo do formulário vai aqui.</p>
        <p>Conteúdo do formulário vai aqui.Conteúdo do formulário vai aqui.</p>
        <p>Conteúdo do formulário vai aqui.Conteúdo do formulário vai aqui.</p>
        <p>Conteúdo do formulário vai aqui.Conteúdo do formulário vai aqui.</p>
        <p>Conteúdo do formulário vai aqui.Conteúdo do formulário vai aqui.</p>
        <p>Conteúdo do formulário vai aqui.Conteúdo do formulário vai aqui.</p>
        
      </ModalProva>
    </div>
  </template>
  
  <script>
  import ButtonAdd from './Button.vue';
  import ModalProva from './ModalProva.vue';
  import { PlusIcon } from '@heroicons/vue/24/solid';
  
  export default {
    name: 'AddProva',
    components: {
      ButtonAdd,
      ModalProva,
      PlusIcon
    },
    data() {
      return {
        isModalVisible: false
      };
    },
    methods: {
      showModal() {
        this.isModalVisible = true;
      }
    }
  }
  </script>
  

  