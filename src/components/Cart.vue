<template>
  <div class="cart">
    <h1>{{title}}</h1>

    <div class="main_cart_switch">
        <h1>{{monthly}}</h1>
        <div class="cart_switch"> 
            <button></button>
        </div>
        <h2>{{yearly}}</h2>
    </div>

    <div class="start_cart">

        <!-- Cart 1 -->
        <div v-for="cart1 in cart1" class="cart1">
            <div class="cat">
                <h3>{{cart1.title}}</h3>
                <h4>{{cart1.description}}</h4>
            </div>
            <div class="cat1">
                <p>{{cart1.price}}<span>{{cart1.month}}</span></p>
            <ul v-for="list in cart1.features">
                <li>{{list}}</li>
            </ul>
            </div>
            <button>{{cart1.first_button}}</button>
        </div>

        <!-- Cart 2 -->
        <div v-for="cart2 in cart2" class="cart2">
            <div class="cat">
                <h3>{{cart2.title}}</h3>
                <h4>{{cart2.description}}</h4>
            </div>
            <div class="cat1">
                <p>{{cart2.price}}<span>{{cart2.month}}</span></p>
            <ul v-for="list in cart2.features">
                <li>{{list}}</li>
            </ul>
            </div>
            <button>{{cart2.second_button}}</button>
        </div>

        <!-- Cart 3 -->

        <div v-for="cart3 in cart3" class="cart3">
            <div class="cat">
                <h3>{{cart3.title}}</h3>
                <h4>{{cart3.description}}</h4>
            </div>
            <div class="cat1">
                <p>{{cart3.price}}<span>{{cart3.month}}</span></p>
            <ul v-for="list in cart3.features">
                <li>{{list}}</li>
            </ul>
            </div>
            <button>{{cart3.third_button}}</button>
        </div>

    </div>
  </div>
</template>

<script>
export default {
data(){
    return{
        title: 'Get your best deal',
        monthly: 'Monthly',
        yearly: 'Yearly',
        cart1: [
            {title:'Personal', 
            description: 'Special first packet for all', 
            price: '$8', 
            month: '/Month',
            features: ['Up to 5 page each group', 'Up to 10 group page', '5 Days group page saved'],
            first_button: 'Start Free Trial'
            }
        ],

        cart2: [
            {title:'Regular', 
            description: 'Recommended for personal pro', 
            price: '$20', 
            month: '/Month',
            features: ['Up to 15 page each group', 'Download page up to 20 page', 'Up to 10 group page', '15 Days group page saved'],
            second_button: 'Start Free Trial'
            }
        ],

        cart3: [
            {title:'Premium', 
            description: 'Packet for Startup & Company', 
            price: '$48', 
            month: '/Month',
            features: ['Unlimited group pages', 'Unlimited download page', 'Unlimited page each group', 'Customize sorting group pages', 
                        'Customize group page name', '30 Days group page saved'],
            third_button: 'Start Free Trial'
            }
        ],
    }

}
}
</script>

<style>
.cart h1{
    color: white;
    text-align: center;
    padding-top: 5%;
    font-size: 80px;
}
.main_cart_switch{
    display: flex;
    margin-left: 40%;
}
.main_cart_switch h1{
    color: white;
    font-size: 25px;   
}
.main_cart_switch h2{
    color: white;
    font-size: 25px;
    padding: 5%;   
}
.cart_switch{
    background-color: white;
    width: 130px;
    height: 60px;
    border-radius: 40px;
    margin-top: 4%;
    margin-left: 4%;
}
.cart_switch button{
    background-color: #A8FF35;
    width: 40px;
    height: 40px;
    border: none;
    border-radius: 20px;
    margin-left: 10px;
    margin-top: 10px;
}
.start_cart{
    margin: 3%;
    display: flex;
    flex-wrap: wrap;
}
.cart1{
    background: #FAFAFA;
    width: 460px;
    height: 600px;
    margin: 3%;
    border-radius: 20px;


}
.cart1 button{
    width: 300px;
    height: 60px;
    margin-left: 15%;
    border-radius: 40px;
    border: none;
    background: #A8FF35;
}

.cart2{
    background: #A8FF35;
    width: 460px;
    height: 600px;
    margin: 3%;
    border-radius: 20px;
}
.cart2 button{
    width: 300px;
    height: 60px;
    margin-left: 15%;
    border-radius: 40px;
    border: none;
    background: black;
    color: white;
}
.cart3{
    background: #FAFAFA;
    width: 460px;
    height: 600px;
    margin: 3%;
    border-radius: 20px;    
}
.cart3 button{
    width: 300px;
    height: 60px;
    margin-left: 15%;
    border-radius: 40px;
    border: none;
    background: #A8FF35;
}
.cat{
    border-bottom: 1px solid black;
    margin: 4% 10%;
    height: 100px;
}
.cat h3{
    font-size: 50px;
}
.cat1{
    padding: 4% 10%;
    height: 320px;
}
.cat1 p{
    font-size: 50px;
    font-weight: bolder;
}
.cat1 span{
    font-size: 20px;
    color: black;
    font-weight: lighter;
}
.cat1 ul{
    padding: 3%;
    margin: 0% 3%;
}
.cat1 ul li{
    font-size: 18px;
}

@media only screen and (max-width: 390px) {
    .cart h1{
        font-size: 40px;
    }
    .cart_switch{
    background-color: white;
    width: 60px;
    height: 40px;
    border-radius: 40px;
    margin-top: 4%;
    margin-left: 4%;
    }
    .cart_switch button{
        width: 20px;
        height: 20px;
    }
    .main_cart_switch{
        margin-left: 20%;
    }
    .main_cart_switch h1{
        font-size: 25px;   
}
    .cart1 button{
        margin-left: 5%;
    }
    .cart2 button{
        margin-left: 5%;
    }
    .cart3 button{
        margin-left: 5%;
    }
}
</style>