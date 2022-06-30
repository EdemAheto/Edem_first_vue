<template>
<div class="join_main">
  <h1>{{title}}</h1>
  <h2>{{title2}}</h2>
  <button>{{title3}}</button>
</div>

</template>

<script>
export default {
    data(){
        return{
            title: 'Join us on email for',
            title2: 'more trending topics',
            title3: 'Join Now '
        }
    }
}
</script>

<style>
    .join_main{
        text-align: center;
        font-size: 50px;
        padding-top: 5%;
        line-height: 120px
    }
    .join_main h2{
        color: #87D322; 
    }
    .join_main button{
        width: 300px;
        height: 60px;
        border-radius: 40px;
        border: none;
        background: black;
        color: white;        
    }

    @media only screen and (max-width: 390px) {
        .join_main{
            font-size: 20px;
            line-height: 60px;
        }
        .join_main button{
            margin-top: 15%;
        }
    }
</style>