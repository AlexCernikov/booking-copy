<template>
<!-- eslint-disable max-len -->
 <section class="admin-nav">
    <div class="container">
      <div class="nav-items">
        <NavBar
      v-for="(item, index) in navBar"
          :key="index"
          :navTitle="item.navTitle"
      />
      </div>
    </div>
 </section>
</template>
<script lang="ts">
import { defineComponent } from 'vue';
import NavBar from '@/components/HomeViewComponents/NavBar.vue';

export default defineComponent({
  components: {
    NavBar,
  },
  data() {
    return {
      navBar: [
        {
          id: 1,
          navTitle: 'Users',
        },
        {
          id: 2,
          navTitle: 'Reservation',
        },
      ],
    };
  },
  name: 'adminNavBar',
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Roboto+Condensed:wght@400;700&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Lato&display=swap');

.container{
    width: 1100px;
    margin: auto;
}
a{
  text-decoration: none;
}
.nav-items{
  display: flex;
  flex-direction: column;
  justify-content: start;
  align-items: center;
}
</style>
