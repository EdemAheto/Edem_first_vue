<template>
<div class="chapter1">
    <h1>{{h2}}</h1>
</div>
<div class="chapter1_content">
    <br>
    <div class="Elon">
        <br>
        <img :src="url">
        <p>{{h4}}</p>
        <div class="cancel">
            <p>{{cancel}}</p>
        </div>
    </div>
</div>
<div class="para">
    <p>{{p}}</p>
    <p>{{p1}}</p>
</div>
</template>

<script>
export default {
data(){
    return{
        h2: 'Open new tabs is sh*t',
        url: require('./assets/logo1.svg'),
        h4:'Findtrend - Elon Musk',
        p: 'A solution for your browser tabs and don’t make your device get slower over time. Get',
        p1: 'ease and faster to discover a trend with just one tab.',
        cancel: 'x'
    }
}
}
</script>

<style>
.chapter1 h1{
    font-size: 80px;
    text-align: center;
    padding-top: 8%;
}
.chapter1_content{
    background: #F5F5F5;
    height: 150px;
    width: 30%;
    margin-left: 35%;
    margin-top: 5%;
    
}
.Elon{
    background-color: black;
    width: 450px;
    height: 80px;
    margin-left: 10%;
    margin-top: 3%;
    display: flex;
}
.Elon img{
    padding-left: 10%;
    width: 60px;
}
.Elon p{
    color: white;
    padding-top: 7%;
    padding-left: 4%;
    font-size: 30px;
}
.para{
    text-align: center;
    font-size: 20px;
    padding-top: 2%;
}
.cancel{
    position: absolute;
    left: 1020px;
    background-image: linear-gradient(to right, rgba(0, 0, 0, 0.567), black);
    width: 125px;
    height: 80px;
}
.cancel p{
    text-align: right;
    padding-top: 20%;
    padding-right: 5%;
}
</style>