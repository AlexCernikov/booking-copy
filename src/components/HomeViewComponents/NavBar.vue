<template>
    <div class="nav" >
      <button>{{navTitle}}</button>
    </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'adminNavBar',
  props: {
    navTitle: {
      type: String,
    },
  },
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
</style>
