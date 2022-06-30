<template>
<header>
  <navigate></navigate>
  <headman></headman>
  <labelman></labelman>  
</header>

<main>
<chap1></chap1>
</main>

<article>
  <chap2></chap2>
</article>

<div class="sponsor">
  <chap3></chap3>
</div>

<div class="main_cart">
  <cart></cart>
</div>

<main class="join">
  <join></join>
</main>

<footer>
  <concluder></concluder>
</footer>

</template>

<script>
import navigate from './components/navigation.vue';
import headman from './components/Header.vue';
import label from'./components/Labels.vue';
import chapter1 from'./components/FirstChapter.vue';
import chapter2 from './components/SecondChapter.vue';
import chapter3 from './components/Sponsor.vue';
import cart from './components/Cart.vue';
import join from './components/Join.vue';
import concluder from './components/Final.vue';
export default {
  name: 'App',
  components: {
    navigate: navigate,
    headman: headman,
    labelman: label,
    chap1: chapter1,
    chap2: chapter2,
    chap3: chapter3,
    cart: cart,
    join: join,
    concluder: concluder,
  }
}
</script>

<style>
*{
  margin: 0;
  padding: 0;
}
header{
  background-color: black;
  height: 100vh;
}
main{
  background-color: #A8FF35;
  height: 80vh;
}
.main_cart{
  margin-top: 10%;
  background-color: black;
  height: 120vh;
}
.join{
  background-color: #A8FF35;
  height: 60vh;
}
footer{
  display: flex;
  justify-content: space-between;
  padding: 1% 5%;
}


@media only screen and (max-width: 390px) {
  .main_cart{
    height: 250vh;
    margin-top: 10%;
  }
  .join{
    height: 35vh;
  }
  footer{
    padding-top: 10%;
    display: block;
  }
}

</style>
