<template>
  <div class="collections">
    <h1>Collections</h1>
    <div class="gallery">
      <div class="item1">
        <div class="desc">
          <h3>XO Girls NFT Collection</h3>
          <p>Floor: 0.07 ETH</p>
        </div>
      </div>
      <div class="item2">
        <div class="desc">
          <h3>Game character 3d Collection</h3>
          <p>Floor: 0.07 ETH</p>
        </div>
      </div>
      <div class="item3">
        <div class="desc">
          <h3>Monkey Collections</h3>
          <p>Floor: 0.07 ETH</p>
        </div>
      </div>
      <div class="item4">
        <div class="desc">
          <h3>PROJECT NFT Cub</h3>
          <p>Floor: 0.07 ETH</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  setup() {
    return {};
  },
};
</script>

<style>
.collections {
  background-color: black;
  /* padding: 50px 70px 5px 5px; */
}
.gallery {
  /* display: flex; */
  justify-content: space-between;
  padding: 20px;
  display: grid;
  grid-template-columns: repeat(4, minmax(0, 1fr));
  gap: 1rem;
}
.item1 {
  background-image: url("../images/Rectangle 13.png");
  background-size: cover;
  width: 100%;
  height: 315px;
  position: relative;
}
.item2 {
  background-image: url("../images/Rectangle 14.png");
  background-size: cover;
  position: relative;
}
.item3 {
  background-image: url("../images/Frame 21.png");
  background-size: cover;
  position: relative;
}
.item4 {
  background-image: url("../images/Rectangle 16.png");
  background-size: cover;
  position: relative;
}
.desc {
  position: absolute;
  background-color: rgba(0, 0, 0, 0.8);
  left: 0;
  bottom: 0;
  width: 100%;
  align-items: center;
  text-align: center;
  height: 65px;
  padding: 3px;
  
}
.desc h3{
  color: white;
 margin: 0;
}

</style>