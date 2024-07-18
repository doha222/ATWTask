<template>
  <navbar class="trans-nav"></navbar>
  <div class="page">
    <div class="postsInfo">
      <ol>
        <li v-for="post in disposts" :key="post.id">
          <h3>{{ post.title }}</h3>
          <p>{{ post.body }}</p>
          <hr />
        </li>
      </ol>
    </div>
  </div>
  <myfooter></myfooter>
</template>
  
  <script>
import navbar from "../components/navbar.vue";
import { ref, onMounted } from "vue";
import axios from "axios";
import Myfooter from '@/components/myfooter.vue';
import myfooter from "@/components/myfooter.vue";
export default {
  components: {
    navbar,
    Myfooter,
  },
  setup() {
    const posts = ref([]);
    const disposts = ref([]);

    onMounted(() => {
      fetchPhotos();
    });

    const fetchPhotos = () => {
      axios
        .get("https://jsonplaceholder.typicode.com/posts")
        .then((response) => {
          posts.value = response.data;
          disposts.value = posts.value.slice(0, 10);
        })
        .catch((error) => {
          console.error(error);
        });
    };

    return {
      posts,
      disposts,
      fetchPhotos,
    };
  },
};
</script>
  <style>
.page {
  background-color: #816797;
  text-align: center;
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 100px 50px;
}
.page .postsInfo {
  text-align: center;
  width: 60%;
}
/* .postsInfo li{
    list-style: none;
} */
</style>
  