<template>
  <div
    class="window-drag flex items-center border-b text-gray-900 border-gray-100"
    style="height: 28px"
  >
    <Fb class="ms-2" />
    <p v-if="companyName && dbPath" class="mx-auto text-sm">
      {{ companyName }} - {{ dbPath }}
    </p>
  </div>
</template>

<script>
import Fb from './Icons/18/fb.vue';

export default {
  name: 'WindowsTitleBar',
  components: { Fb },
  props: {
    dbPath: String,
    companyName: String,
  },
};
</script>
