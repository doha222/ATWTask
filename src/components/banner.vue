<template>
  <div class="banner">
    <div class="content">
      <h1>Your own NFT Market place without Coding</h1>
      <p>
        The fastest and easiest way to fully unlock the potential of your
        digital assets. Create and run an exclusive marketplace for your NFT
        business today!
      </p>
      <div class="info">
        <input type="text" placeholder="Enter Your Email..." />
        <button @click="goToPosts">Start Free</button>
      </div>
      <button @click="goToPosts">Show Posts</button>
    </div>
  </div>
  <div class="smallFooter">
    <p>Powering leading brands</p>
    <div>
      <img src="../images/Frame 10.png" alt="" />
      <p>Coindesk</p>
    </div>
    <div>
      <img src="../images/Frame 7.png" alt="" />
      <p>H E F T Y V E R S E</p>
    </div>
  </div>
</template>
  
  <script>
import { useRoute, useRouter } from "vue-router";
import { ref } from "vue";
export default {
  setup() {
    const route = useRoute();
    const router = useRouter();

    const goToPosts = () => {
      router.push({ name: "page" });
    };

    return {
      goToPosts,
    };
  },
};
</script>
  
<style>
.banner {
  background-image: url("../images/Home\ Background.png");
  background-size: cover;
  width: 100%;
  height: 100vh;
  background-position: center;
  background-repeat: no-repeat;
  background-color: rgba(0, 0, 0, 0.9);
  align-items: center;
}
.content {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  padding: 20px;
  text-align: center;
}
h1 {
  font-size: 48px;
  font-weight: 700px;
  line-height: 72px;
  color: white;
}
p {
  color: white;
  font-size: 17px;
  font-weight: 400px;
}
input {
  background-color: rgba(0, 0, 0, 0.7);
  border-radius: 30px;
  width: 270px;
  align-items: center;
  padding: 2px;
  height: 35px;
  box-sizing: border-box;
  line-height: 1.42857;
  padding: 8px 6px;
  border: none;
}
.info {
  display: flex;
  align-content: center;
  text-align: center;
  margin-left: 100px;
  margin-bottom: 15px;
}
.info button {
  width: 84px;
  height: 37px;
  border-radius: 30px;
  background-color: #52057b;
  margin-right: 15px;
  font-weight: bold;
  color: white;
  border: none;
  line-height: 30px;
  font-weight: 400px;
}
.content > button {
  border-radius: 30px;
  background-color: #52057b;
  margin-right: 15px;
  font-weight: bold;
  color: white;
  border: none;
  line-height: 30px;
  font-weight: 400px;
  width: 40%;
  transition: 0.5s;
}
.content > button:hover {
  width: 60%;
  color: #52057b;
  font-weight: 500px;
  font-size: 18px;
  background-color: white;
  cursor: pointer;
}
.smallFooter {
  background-color: #816797;
  display: flex;
  justify-content: space-around;
  height: 83px;
  text-align: center;
  align-items: center;
}
.smallFooter img {
  width: 65px;
  height: 45px;
}
.smallFooter div {
  display: flex;
  text-align: center;
  align-items: center;
}
</style>


