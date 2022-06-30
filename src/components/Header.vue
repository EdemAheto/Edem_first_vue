<template>
<div class="title">
  <h1>{{title}}</h1>
  <h1>{{title1}}</h1>
  <p>{{p}}</p>
  <p>{{p1}}</p>
  <button>{{started}}</button>
</div>
</template>

<script>
export default {
data (){
    return{
        title: 'Minimize your tabs.',
        title1: 'Find the trends!',
        p: 'Don’t let your computer memories consumes all of those browser tabs.',
        p1: 'Findtrend  let you gathers all of your favorite website into one place.',
        started: 'Get Started 🔥'

    }
}
}
</script>

<style>
.title{
    padding-top: 8%;
}
.title h1{
    color: white;
    text-align: center;
    font-size: 90px;
}
.title p{
    color: #8B8B8B;
    text-align: center;
    font-size: 25px;
}
.title button{
    width: 250px;
    height: 60px;
    margin-left: 45%;
    margin-top: 3%;
    border-radius: 40px;
    background: #A8FF35;

}
</style>