<template>
<div class="first_main_label">


<div class="labels" v-for="label in label">
    <div class="main_label">
        <img :src="label.url">
        <p>{{label.title}}</p>
        <div class="cancels">
            <p>{{label.cancel}}</p>
        </div>
    </div>
  </div>

    <div class="labels" v-for="label1 in label1">
    <div class="main_label1">
        <img :src="label1.url">
        <p>{{label1.title}}</p>
        <div class="cancels1">
            <p>{{label1.cancel}}</p>
        </div>
    </div>
  </div>

    <div class="labels" v-for="label2 in label2">
    <div class="main_label2">
        <img :src="label2.url">
        <p>{{label2.title}}</p>
        <div class="cancels2">
            <p>{{label2.cancel}}</p>
        </div>
    </div>
  </div>

    <div class="labels" v-for="label3 in label3">
    <div class="main_label3">
        <img :src="label3.url">
        <p>{{label3.title}}</p>
        <div class="cancels3">
            <p>{{label3.cancel}}</p>
        </div>
    </div>
  </div>

</div>
  

</template>

<script>
export default {
data(){
    return{
        label:[
            {url: require('./assets/twitter.svg'), title: 'Cryptopunk - Search', cancel:'x'},
        ],
        label1: [
            {url: require('./assets/Pinterest.svg'), title: 'Popular Design - Search', cancel:'x'},
        ],
        label2: [
            {url: require('./assets/facebook.svg'), title: 'Product Design - Search', cancel:'x'},
        ],
        label3: [
            {url: require('./assets/Elon.svg'), title: 'Elon Musk - Search', cancel:'x'}
        ]
    }
}
}
</script>

<style>
.main_label{
    color: white;
    display: flex;
    width: 341.23px;
    height: 82px;
    position: absolute;
    left: 226px;
    top: 654.8px;
    background: #181818;
    transform: rotate(-4deg);
    z-index: 4;
    margin-left: 5%;
}
.main_label p{
    padding-top: 8%;
    font-size: 25px;
}
.main_label1{
    color: white;
    display: flex;
    width: 341.23px;
    height: 82px;
    position: absolute;
    left: 531.16px;
    top: 699.47px;
    background: #181818;
    transform: rotate(2deg);
    z-index: 3;
    margin-left: 5%;
}
.main_label1 p{
    padding-top: 8%;
    font-size: 25px;
}
.main_label2{
    color: white;
    display: flex;  
    width: 341.23px;
    height: 82px;
    position: absolute;
    left: 850.12px;
    top: 657.78px;
    background: #181818;
    transform: rotate(-2deg);
    z-index: 2;
    margin-left: 5%;
}
.main_label2 p{
    padding-top: 8%;
    font-size: 25px;
}
.main_label3{
    color: white;
    display: flex;
    width: 341.23px;
    height: 82px;
    left: 1163.6px;
    position: absolute;
    top: 695.13px;
    background: #181818;
    transform: rotate(4deg);
    z-index: 1;
    margin-left: 5%;
}
.main_label3 p{
    padding-top: 8%;
    font-size: 25px;
}
.first_main_label{
    height: 30vh;
    margin-left: 5%;
    padding-left: 12%;
}
.cancels{
    z-index: 1;
    position: absolute;
    left: 230px;
    width: 110px;
    height: 82px;
    text-align: center;
    background-image: linear-gradient(to right, rgba(0, 0, 0, 0.83), black);
}
.cancels p{
    padding-top: 20%;
    padding-right: 5%;
}
.cancels1{
    z-index: 1;
    position: absolute;
    left: 230px;
    width: 110px;
    height: 82px;
    text-align: center;
    background-image: linear-gradient(to right, rgba(0, 0, 0, 0.83), black);
}
.cancels1 p{
    padding-top: 20%;
    padding-right: 5%;
}
.cancels2{
    z-index: 1;
    position: absolute;
    left: 230px;
    width: 110px;
    height: 82px;
    text-align: center;
    background-image: linear-gradient(to right, rgba(0, 0, 0, 0.83), black);
}
.cancels2 p{
    padding-top: 20%;
    padding-right: 5%;
}
.cancels3{
    z-index: 1;
    position: absolute;
    left: 230px;
    width: 110px;
    height: 82px;
    text-align: center;
    background-image: linear-gradient(to right, rgba(0, 0, 0, 0.83), black);
}
.cancels3 p{
    padding-top: 20%;
    padding-right: 5%;
}

</style>