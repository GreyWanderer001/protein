<script>
export default {
  data() {
    return {
      products: [
        { id: 1, name: "", price: "Protein shakes are essential for muscle recovery and growth after a tough workout."},
        { id: 2, name: "", price: "Creatine boosts strength and power, perfect for weightlifting and high-intensity workouts."},
        { id: 11, name: "", price: "Casein protein before bed aids in overnight muscle recovery and growth."},
        // Add more product objects as needed
      ],
    };
  },
};
</script>

<template>

    <div id="container">
        <p class="eat">Eat good, look good</p>
        <div class="text">Welcome to PowerFuel Provisions, your one-stop online shop for premium sports nutrition supplements and fuel for athletes and fitness enthusiasts. Discover a wide selection of high-quality protein
    powders, amino acids, vitamins, performance enhancers, and more to help you reach your fitness 
    goals and unleash your inner strength. We strive to provide exceptional products from trusted 
    brands, ensuring you get the nutrients you need to optimize your performance and recovery. Elevate
    your fitness journey with PowerFuel Provisions, where power meets performance</div>
            <a href="/product">
            <button class="button">Shop now</button>
        </a>

    

    </div>

    <img src="../components/protein.png" alt="Your Image" class="img">

    

    <div>
    <p class="eat2">Testimonials</p>
    </div>

    <div class="wrapper">
      <div class="square" v-for="product in products" :key="product.id">
        <div class="description">
          <a class="text">{{ product.name }}</a>
          <p class="text">{{ product.price }}</p>
        </div>
      </div>
    </div>

    

</template>

<style scoped>

.wrapper {
        display:flex;
        justify-content:center;
        align-items:center;
        flex-wrap:wrap;
        flex-direction:row;
        gap:20px 20px;
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

    .eat{
        color: #ffffff;
        font-family: Inter;
        font-size: 50px;
        font-style: normal;
        font-weight: 900;
        line-height: normal;
        letter-spacing: 2px;
    }

    .eat2{
        color: #ffffff;
        font-family: Inter;
        font-size: 50px;
        font-style: normal;
        font-weight: 900;
        line-height: normal;
        letter-spacing: 2px;
        text-align: center;
        margin-top:500px;
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

    .button {
        width: 187px;
        height: 88px;
        flex-shrink: 0;
        border-radius: 20px;
        background: #FFB800;
        box-shadow: 0px 4px 4px 0px rgba(0, 0, 0, 0.25);
        border: none;
        cursor: pointer;
        font-size: 24px;
        font-weight: bold;
        color: black;
        margin-top:40px;
    }
.center-container {
  text-align: center;
}
</style>