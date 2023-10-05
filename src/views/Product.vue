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

    <div></div>



</template>

<style >

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