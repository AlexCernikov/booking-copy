<template>
    <div class="nav">
      <button class="btn-nb" @click="show">{{navTitle}}</button>
    </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import AdminUsers from './AdminUsers.vue';

export default defineComponent({
  component: {
    AdminUsers,
  },
  data() {
    return {
      ev: 1,
    };
  },
  name: 'adminNavBar',
  props: {
    navTitle: {
      type: String,
    },
  },
  // methods: {
  //   show() {
  //     console.log('show');
  // },
  //   },
  // },
});
</script>
<style scoped lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Roboto+Condensed:wght@400;700&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Lato&display=swap');
.container{
    max-width: 1100px;
    margin: auto;
}
a{
  text-decoration: none;
}
.btn-nb{
  background: royalblue;
  margin-bottom: 15px;
}
</style>
