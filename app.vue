<script setup>
import { ref } from 'vue';
import { render } from '@vue-email/render';

import Email from './components/Email.vue';

const plainText = ref('');

const onRender = async () => {
  console.log('onRender');
  plainText.value = await render(Email);
  console.log('plainText.value', plainText.value);
};
</script>

<template>
  <button @click="onRender">Render</button>
  {{ plainText }}
</template>
