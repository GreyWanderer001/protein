<script>
  
</script>

<template>

    <div id="container">
        <p class="eat">Eat good, look good</p>
        <div class="text">Welcome to PowerFuel Provisions, your one-stop online shop for premium sports nutrition supplements and fuel for athletes and fitness enthusiasts. Discover a wide selection of high-quality protein
    powders, amino acids, vitamins, performance enhancers, and more to help you reach your fitness 
    goals and unleash your inner strength. We strive to provide exceptional products from trusted 
    brands, ensuring you get the nutrients you need to optimize your performance and recovery. Elevate
    your fitness journey with PowerFuel Provisions, where power meets performance</div>
    </div>
    <img src="../components/protein.png" alt="Your Image" class="img">

</template>

<style scoped>
    .eat{
        color: #ffffff;
        font-family: Inter;
        font-size: 50px;
        font-style: normal;
        font-weight: 900;
        line-height: normal;
        letter-spacing: 2px;
    }

    .text{
        color: #FFB800;
        font-family: Inter;
        font-size: 15px;
    }

    #container{
        display: flex;
        align-items: left;
        flex-direction: column;
        position: absolute;
        left: 10%;
        width: 40%;
    }
    .img{
        width: 398px;
        height: 530px;
        position: absolute;
        right:0;

    }

    @media screen and (max-width: 500px) {
        .img {
            width: 200px;
            height: 300px;

        }
    }
</style>