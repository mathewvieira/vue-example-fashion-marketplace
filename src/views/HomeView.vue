<script setup lang="ts">
import Logo from '@/assets/img/logo/logo.png'
import BannerImg from '@/assets/img/banner/banner.png'
</script>

<template>
  <main>
    <header>
      <div class="logo">
        <img :src="Logo" alt="" />
      </div>

      <nav>
        <ul>
          <li>CATALOGUE</li>
          <li>FASHION</li>
          <li>FAVORITE</li>
          <li>LIFESTYLE</li>
        </ul>

        <button>SIGN UP</button>
      </nav>
    </header>

    <section class="banner">
      <div class="text">
        <h1>LET'S<br />EXPLORE<br /><span>UNIQUE</span><br />CLOTHES</h1>
        <h3>Lorem ipsum dolor sit amet consectetur adipisicing elit.</h3>
        <button>SEE MORE</button>
      </div>

      <div class="img">
        <img :src="BannerImg" alt="" />
      </div>
    </section>
  </main>
</template>

<style scoped>
main {
  width: 1290px;
  margin: 0 auto;
}

main header {
  display: flex;
  justify-content: space-between;
}

main header nav {
  display: flex;
  align-items: center;
  gap: 55px;
}

main header nav ul {
  padding: 0;
  display: flex;
  gap: 60px;
}

main header nav ul li {
  list-style: none;
  padding: 0;
  font-size: 20px;
}

main header nav button {
  padding: 8px 12px;
  background-color: black;
  border-radius: 6px;
  color: white;
  cursor: pointer;
}

main header nav button:hover {
  background-color: white;
  color: black;
}

main .banner {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #f4f6f5;
  border-radius: 60px;
  padding: 10px 70px 0 70px;
}

main .banner .text h1 {
  font-weight: 900;
  font-size: 60px;
  padding: 0;
  margin: 0;
}

main .banner .text h1 span {
  font-weight: 900;
  position: relative;
  transform: rotate(-2deg);
}

main .banner .text h1 span:before {
  content: '';
  position: absolute;
  width: 115%;
  height: 90%;
  top: 4.5%;
  left: -7%;
  z-index: -1;
  background-color: yellow;
  transform: rotate(-2deg);
}

main .banner .text h3 {
  font-size: 18px;
  padding: 0;
  margin: 0;
}

main .banner .text button {
  padding: 8px 40px;
  margin: 20px 0;
  background-color: white;
  border-radius: 6px;
  color: black;
  cursor: pointer;
  font-size: 20px;
}

main .banner .img {
  width: 55%;
}

main .banner .img img {
  width: 100%;
}
</style>
