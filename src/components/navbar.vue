<template>
  <nav>
    <div>
     <a href=""><img @click="goToHome" src="../images/logo.png" alt="" /></a> 
    </div>
    <div class="links">
      <ul>
        <a href="" @click="goToHome"><li>Home</li></a>
        <a href=""><li>About</li></a>
        <a href=""><li>Blog</li></a>
        <a href=""><li>Cart</li></a>
      </ul>
      <div class="btns">
        <button class="log">login</button>
        <button class="sign">signup</button>
      </div>
    </div>
  </nav>
</template>

<script>
import { useRoute, useRouter } from "vue-router";
export default {
  setup() {
    const router = useRouter();
    const goToHome = () => {
      router.push({ name: "home" });
    };
    return {
      goToHome,
    };
  },
};
</script>

<style>
nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: rgba(0, 0, 0, 0.5);
  padding: 3px 10px;
}
.links {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.links ul {
  list-style: none;
  display: flex;
  justify-content: flex-end;
  align-items: center;
  gap: 10px;
  color: white;
  line-height: 30px;
  font-weight: 400px;
}
.links ul a {
  text-decoration: none;
}
.links ul li {
  color: white;
  padding: 5px 10px;
  border-radius: 5px;
}
.btns {
  margin-left: 30px;
  display: flex;
  justify-content: space-between;
}
.btns button {
  width: 84px;
  height: 37px;
  border-radius: 30px;
  margin-right: 15px;
  font-weight: bold;
  /* color: white; */
  line-height: 30px;
  font-weight: 400px;
}
.sign {
  background-color: #52057b;
  border: none;
}
.log{
  background-color: rgba(0, 0, 0, 0.3);
  color: white;
  border-color: #52057b;
}
</style>