<template>
  <div class="home">
    <AdminNavBar />
ADMIN
  </div>
</template>

<script lang="ts">

import { defineComponent } from 'vue';
import AdminNavBar from '@/components/HomeViewComponents/AdminNavBar.vue';

export default defineComponent({

  name: 'app',
  components: {
    AdminNavBar,
  },
});
</script>
