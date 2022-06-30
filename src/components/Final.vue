<template>
  <div class="main_final">
    <img :src="url">
    <h1>{{name}}</h1>
  </div>
  <div v-for="links in links" class="footer_nav">
    <li>{{links}}</li>
  </div>

</template>

<script>
export default {
    data(){
        return{
            url: require('./assets/Footer_logo.svg'),
            name:'Findtrend',
            links: ['Privacy Policy', 'Terms and Conditions', 'Contact Us', 'Careers']
        }
    }
}
</script>

<style>
    .main_final{
        display: flex;
        width: 900px;
    }
    .footer_nav{
        width: 150px;
    }

    .footer_nav li{
        list-style-type: none;
        text-align: center;

    }
    @media only screen and (max-width: 390px) {
        .main_final{
            width: 200px;
            margin-left: 25%;
            margin-top: 5%;
        }
        .footer_nav{
            margin: 10% 30%;
        }
    }

</style>