<template>
  <div class="sponsorship">
    <br>
    <h2>{{h6}}</h2>
</div>
 
<div class="sponsor_list">
        <li v-for="url_sponsor in url_sponsor">
        <div class="spon">
            <img :src="url_sponsor">
        </div>
    </li>
</div>

<div class="main_collaboration">
    <h2>{{collaboration_title}}</h2>
<div class="collaboration">
    <ul v-for="collaboration in collaboration">
        <li>
            <img :src="collaboration">
        </li>
    </ul>
</div>
</div>

<div class="tweet">
    <ul v-for="tweets in tweets">
        <li><img :src="tweets"></li>
    </ul>
<button>{{trend}}</button>
</div>


</template>

<script>
export default {
data(){
    return{
        h6: 'Findtrend make +1000 Startup grow',
       url_sponsor: [require('./assets/Microsoft.svg'), require('./assets/Alliaz.svg'), require('./assets/Upwork.svg'), require('./assets/Volvo.svg'),
                    require('./assets/Grab.svg'), require('./assets/Verizon.svg'), require('./assets/Coinbase.svg'),require('./assets/Expedia.svg'), 
                    require('./assets/Airtable.svg'), require('./assets/Magento.svg'), require('./assets/Carrera.svg'), require('./assets/Bonanza.svg'),
                    require('./assets/Wetransfer.svg'), require('./assets/Suzuki.svg'), require('./assets/Algolia.svg'), require('./assets/Heineken.svg')
       ],
       collaboration_title: 'All platform connect to Findtrend',
       collaboration: [require('./assets/facebook.svg'), require('./assets/twitter.svg'), require('./assets/Elon.svg'), require('./assets/Pinterest.svg'),
                        require('./assets/Mega.svg'), require('./assets/Reddit.svg'), require('./assets/Vk.svg'), require('./assets/Linkedin.svg')
       ],
       tweets: [require('./assets/tweet 1.svg'), require('./assets/tweet 2.svg'), require('./assets/tweet 3.svg')],
       trend: 'View More Trend',
    }
}
}
</script>

<style>
    .sponsorship{
        margin-top: 15%;
        font-size: 45px;
        text-align: center;
    }
    .sponsorship img{
        margin-top: 5%;
    }
    .sponsor_list{
        display: flex;
        flex-wrap: wrap;
        padding: 5% 10%;
        
    }
    .sponsor_list li{
        padding: 3% 6%;
        list-style-type: none;
        background: #F5F5F5;
        margin: 1%;
        width: 150px;
        height: 50px;
        border-radius: 20px;
    }
    .main_collaboration{
        text-align: center;
        font-size: 45px;
        padding-top: 6%;
    }
    .collaboration{
        display: flex;
        flex-wrap: wrap;
        padding-left: 18%;
        padding-top: 6%;
    }
    .collaboration ul{
        text-align: center;
        padding: 2.5%;
    }
    .collaboration ul li{
        list-style-type: none;
    }
    .collaboration ul li img{
        width: 70px;
        height: 70px;
    }
    .tweet{
        padding-top: 10%;
        padding-left: 27%;
    }

    .tweet ul li{
        list-style-type: none;
        padding-top: 5%;
    }
    .tweet button{
        margin-top: 5%;
        width: 250px;
        height: 50px;
        border-radius: 40px;
        background-color: black;
        color: white;
        margin-left: 20%;
    }

@media only screen and (max-width: 390px) {
    .main_collaboration{
        font-size: 30px;
        padding-top: 6%;
    }
    .collaboration{
        padding-left: 5%;
    }
    .collaboration ul li img{
        width: 40px;
        height: 40px;
    }
    .tweet{
        padding-left: 10%;
    }
    .tweet ul li img{
        width: 300px;
    }
    .tweet button{
        margin-left: 8%;
    }
}
</style>