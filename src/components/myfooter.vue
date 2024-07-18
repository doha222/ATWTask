<template>
  <div class="container">
    <div class="footer">
      <div class="sub">
        <h2>Join our weekly digest!</h2>
        <p>Get exclusive promotions & updates straight to your inbox.</p>
        <input type="text" placeholder="Enter your email..." />
        <button class="btn1">Subscribe</button>
        <br />
        <button class="btn2">Create free store now</button>
      </div>
      <div class="link">
        <div>
          <h4>FEATURES</h4>
          <ul>
            <li>Build Store</li>
            <li>Sell NFT</li>
            <li>Grow Business</li>
          </ul>
        </div>
        <div>
          <h4>SERVICES</h4>
          <ul>
            <li>Concierge</li>
            <li>Customization</li>
          </ul>
        </div>
        <div>
          <h4>PRODUCT</h4>
          <ul>
            <li>About Us</li>
            <li>Whitepaper</li>
            <li>$N1 Token</li>
            <li>Directory</li>
          </ul>
        </div>
        <div>
          <h4>RESOURCES</h4>
          <ul>
            <li>Help Center</li>
            <li>NFTify Branding</li>
            <li>Success Stories</li>
            <li>Success Stories</li>
            <li>Video Tutorials</li>
            <li>Contact Support</li>
          </ul>
        </div>
      </div>
    </div>
    <hr />
    <div class="foot">
      <h3>The Leading No-code NFT Marketplace Solution</h3>
      <div class="contentt">
        <div class="copyright">
          <span>&#169;</span>
          <p>Copyright NFTify Network. All Rights Reserved.</p>
        </div>
        <div class="icons">
          <ul>
            <li>
              <a href=""><img src="../images/twitter.png" alt="" /></a>
            </li>
            <li>
              <a href=""><img src="../images/telegram.png" alt="" /></a>
            </li>
            <li>
              <a href=""><img src="../images/facebook.png" alt="" /></a>
            </li>
            <li>
              <a href=""><img src="../images/linkedin.png" alt="" /></a>
            </li>
            <li>
              <a href=""><img src="../images/youtube.png" alt="" /></a>
            </li>
            <li>
              <a href=""><img src="../images/instagram.png" alt="" /></a>
            </li>
          </ul>
        </div>
        <div class="Terms">
          <ul>
            <li><a href="">Terms of Services</a></li>
            <li><a href="">Privacy Policy</a></li>
          </ul>
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

<style >
.container {
  background-image: linear-gradient(#52057b, #000000);
}
.footer {
  display: flex;
  justify-content: space-around;

  padding: 20px;
}
.footer h2 {
  color: white;
}
.sub {
  width: 385px;
}
.footer h4 {
  color: white;
  text-align: center;
}
.footer .btn2 {
  border-radius: 30px;
  background-color: #52057b;
  margin-right: 15px;
  font-weight: bold;
  color: white;
  border: none;
  line-height: 30px;
  font-weight: 400px;
  margin: 10px;
}
.btn1 {
  background-color: black;
  color: white;
  border-color: #52057b;
  line-height: 30px;
  font-weight: 400px;
  border-radius: 30px;
}
.footer .link {
  display: grid;
  grid-template-columns: repeat(4, minmax(0, 1fr));
  gap: 1rem;
  color: white;
}
.link li {
  list-style: none;
  color: #d6d5a8;
  font-size: 12px;
  line-height: 30px;
  margin: 8px;
}
hr {
  color: #816797;
  height: 2px;
  border: none;
  background-color: #816797;
}
.foot h3 {
  color: white;
  text-align: center;
}

.copyright span {
  content: "\00A9";
  color: white;
  padding-top: 18px;
  margin-right: 5px;
  margin-bottom: 16px;
}
.contentt {
  display: flex;
  justify-content: space-around;
}
.copyright {
  display: flex;
  align-items: center;
}
.copyright p {
  font-size: 12px;
  line-height: 18px;
  font-weight: 400px;
}
.icons ul {
  display: flex;
}
.foot li {
  list-style: none;
}
.foot h3{
  font-weight: 500px;
  font-size: 20px;
  line-height: 30px;
}
.icons img {
  border-radius: 30%;
  border-color: white;
  border-width: 80px;
  margin-right: 15px;
  padding: 10px;
}
.Terms ul {
  display: flex;
}

.Terms a {
  color: white;
  text-decoration: none;
  margin-right: 5px;
  font-size: 12px;
  line-height: 18px;
  font-weight: 400px;
}
</style>