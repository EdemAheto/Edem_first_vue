<template>
<div class="article">
    <h1>{{h1}}</h1>
    <h1>{{h2}}</h1>
    <h1>{{h3}} <span>{{h4}}</span></h1>
    <h1><span>{{h5}}</span></h1>
</div>

</template>

<script>
export default {
data(){
    return{
        h1: 'Findtrend helps you to increase your ',
        h2: 'productivity and reduce your computer\'s',
        h3: 'memory load,',
        h4: 'an application that can',
        h5: 'fulfill your daily browsing needs.',
    }
}
}
</script>

<style>
    article{
        padding-top: 5%;
        padding-left: 16%;
        font-size: 45px;
        line-height: 101px;
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        font-weight: lighter;
    }

    span{
        color: #ADADAD;
    }

</style>