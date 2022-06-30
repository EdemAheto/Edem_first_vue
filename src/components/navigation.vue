<template>
  <section>

    <div class="logo">
      <img :src="url">
      <h3>{{logoName}}</h3>
    </div>

    <ul v-for="item in nav">
      <li>{{item}}</li>
    </ul>

    <div class="register">
      <a :href="log">Login</a>
      <button>{{signup}}</button>

    </div>
  </section>
</template>

<script>
export default {
data (){
  return {
    logoName: 'Findtrend',
    nav: ['About', 'How it work', 'Pricing', 'Solution', 'Features'],
    url: require('./assets/logo1.svg'),
    signup: 'Register',
    log: '#'
    
  }
}
}
</script>

<style>
section{
  display: flex;
  justify-content: space-between;
}
.logo h3{
  color: white;
  font-size: 40px;
}
.logo{
  display: flex;
  width: 300px;
  padding: 0.5%;
}
section ul{
  padding: 1%;
  font-size: 20px;
}
section ul li{
  color: white;
  text-decoration: none;
  list-style-type: none;
  
}
section img{
  width: 60px;
  height: 60px;
}
.register button{
  width: 129px;
  height: 42px;
  background: #FFFFFF;
  border-radius: 40px;
  margin-left: 20%;
  margin-top: 5%;
}
.register a{
  margin-left: 1%;
  color: white;
  padding-top: 8%;
  font-size: 20px;
  text-decoration: none;
}
.register{
  width: 15%;
  display: flex;
}
</style>