<script>
  
</script>

<template>

    <h5 class="product">ALL PRODUCTS</h5>
    <div class="container">
        <div class="cat">
            <a>PRICE</a>
            <button><img class="photo" src="../components/strelka.png"></button>
            <a>CATEGORY</a>
            <button><img class="photo" src="../components/strelka.png"></button>
        </div>
        
    </div>

    <div class="wrapper">
        <div class="square" v-for="item in [1,2,3,4,5,6,7,8,9,10,11,12]">
            <img src="../components/protein.png" alt="Your Image" class="img">
        </div>
    </div>
   



</template>

<style >

    .wrapper {
        display:flex;
        justify-content:center;
        align-items:center;
        flex-wrap:wrap;
        flex-direction:row;
        gap:20px 20px;
    }

    .img{
        width: 104px;
        height: 152px;
        flex-shrink: 0;
        margin: auto;
    }

    .square{
        
        display:flex;
        justify-content:center;
        align-items:center;
        width: 258px;
        height: 233px;
        border-radius: 20px;
        background: rgba(255, 255, 255, 0.01);
        box-shadow: 0px 4px 4px 0px rgba(0, 0, 0, 0.25), 0px 4px 4px 0px rgba(0, 0, 0, 0.25) inset;
    }

    .container {
        margin-top: -80px;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .photo{
        width: 25px;
        height: 25px;
        transform: rotate(90deg);
        align-items: center;
    }

    .cat{
        margin-bottom: 100px;
        color: #ffffff;
        font-family: Inter;
        font-size: 15px;
        font-style: normal;
        font-weight: 700;
        line-height: normal;
        letter-spacing: 1px;
        text-align: center;
        display: flex;
        justify-content: center;    
        align-items: center;
        gap: 20px;
    }
    
    .product{
        text-align: center;
        color: #ffffff;
        font-family: Outfit;
        font-size: 50px;
        font-style: normal;
        font-weight: 900;
        line-height: normal;
        letter-spacing: 2px;
    }
</style>