<script>
  
</script>

<template>
  <div>
    <h5 class="product">ALL PRODUCTS</h5>

    <div class="container">
      <div class="cat">
        <a >PRICE</a>
        <button @click="sortByPrice"><img class="photo" src="../components/strelka.png"></button>
        <a >NAME</a>
        <button @click="sortByName"><img class="photo" src="../components/strelka.png"></button>
      </div>
    </div>

    <div class="wrapper">
      <div class="square" v-for="product in filteredProducts" :key="product.id">
        <div class="description">
          <img :src="product.image" alt="Product Image" class="img">
          <a class="text">{{ product.name }}</a>
          <p class="text">Price: {{ product.price }}€</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      products: [
        { id: 1, name: "Optimum Nutrition", price: 20, image: "src/components/protein.png" },
        { id: 2, name: "Protein", price: 30, image: "src/components/protein.png" },
        { id: 3, name: "Creatin Nutrition", price: 15, image: "src/components/b.webp" },
        { id: 4, name: "Creatin Nutrition", price: 15, image: "src/components/b.webp" },
        { id: 5, name: "Creatin Nutrition", price: 15, image: "src/components/b.webp" },
        { id: 6, name: "Creatin Nutrition", price: 15, image: "src/components/b.webp" },
        { id: 7, name: "Trenbolon Nutrition", price: 10, image: "src/components/e.png" },
        { id: 8, name: "Trenbolon Nutrition", price: 10, image: "src/components/e.png" },
        { id: 9, name: "Optimum Nutrition", price: 5, image: "src/components/protein.png" },
        { id: 10, name: "Optimum Nutrition", price: 130, image: "src/components/protein.png" },
        { id: 11, name: "Optimum Nutrition", price: 200, image: "src/components/protein.png" },
        // Add more product objects as needed
      ],
      sortBy: "default", // "default", "price", or "name"
    };
  },
  computed: {
    filteredProducts() {
      if (this.sortBy === "price") {
        return [...this.products].sort((a, b) => a.price - b.price);
      } else if (this.sortBy === "name") {
        return [...this.products].sort((a, b) => a.name.localeCompare(b.name));
      }
      return this.products;
    },
  },
  methods: {
    sortByPrice() {
      this.sortBy = "price";
    },
    sortByName() {
      this.sortBy = "name";
    },
    // ... other methods
  },
};
</script>


<style scoped>

    .description{
        display:flex;
        justify-content:center;
        flex-direction:column;
        align-items:center;

    }

    .text{
        color: #FFB800;
        font-family: Inter;
        font-size: 10px;
        font-style: normal;
        font-weight: 700;
        line-height: normal;
        letter-spacing: 0.4px;
        align-items: bottom;
    }

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