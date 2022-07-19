// <template>
// Hello
//   <div v-for="value in post"
//   :key="value"
//   :email="value.email">
//   <h3>{{email}}</h3>
//   console.log({{email}})
//   </div>
// </template>

// <script lang="ts">
// import { defineComponent } from 'vue';
// import axios from 'axios';

// export default defineComponent({
//   name: 'testView',
//   data() {
//     return {
//       post: [],
//     };
//   },
//   mounted() {
//     axios.get('https://reqres.in/api/users?page=2')
//       .then((res) => {
//         this.post = res.data;
//       });
//   },
// });
// </script>
