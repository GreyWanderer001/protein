<script setup>

</script>

<template>
    <link href='https://fonts.googleapis.com/css?family=Outfit' rel='stylesheet'>
    <link href='https://fonts.googleapis.com/css?family=Inter' rel='stylesheet'>
    
    <header>
        <div class="navigator">
            <div class="navigator2">
                <a class="logo" href="/">FitFuel</a>

                <div class="routes">
                <a href="/home">Home</a>
                <a href="/product">Product</a>
                <a href="/about">About</a>
                </div>
            </div>
        </div>
    </header>
  
</template>

<style scoped>


    template{
        background: #222;
            width: 1920px;
            height: 74px;
            flex-shrink: 0;
    }

    .Home{
        color: #FFF;
        display: flex;
        width: 71px;
        height: 23px;
        font-size: 15px;
        padding-right: 0px;
        align-items: center;
        flex-shrink: 0;
        padding-right: 10px;
    }

    .Product{
        color: #FFF;
        font-family: Outfit;
        font-size: 15px;
        font-style: normal;
        font-weight: 400;
        line-height: 23px; /* 92% */
    }
    .About{
        color: #FFF;
        font-family: Outfit;
        font-size: 15px;
        font-style: normal;
        font-weight: 400;
        line-height: 23px; /* 92% */
    }

    header {
         padding: 0 20px;
      }

      .navigator {
         display: flex;
         justify-content: flex-start;
         align-items: center;
      }


    .navigator2 {
         width: 40%;
         display: flex;
         justify-content: space-between;
         align-items: center;
         flex-direction: row;
    }

    .routes {
        color: #FFF;
         display: flex;
         justify-content: center;
         align-items: center;
         gap:40px;
         flex-direction: row;

      }

      a{
        font-family: Outfit;
        text-decoration: none;
        outline: none;
        color: inherit;
      }

      .logo{
        color: #FFF;
        font-family: Outfit;
        font-size: 25px;
        font-style: normal;
        font-weight: 400;
        line-height: normal;
        margin-right: 30px;
      }
</style>