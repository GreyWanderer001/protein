<template>
    <link href='https://fonts.googleapis.com/css?family=Gochi Hand' rel='stylesheet'>
    <link href='https://fonts.googleapis.com/css?family=Inter' rel='stylesheet'>
    <p class="autumn">Autumn set</p>
    <p class="high">HIGH PROTEIN</p>
    <p class="sale">SALE</p>
    <div class="point">
        <svg xmlns="http://www.w3.org/2000/svg" width="28" height="100" viewBox="0 0 28 100" fill="none">
            <rect width="9.33333" height="10" rx="4.66667" fill="white"/>
            <rect y="15.0002" width="9.33333" height="10" rx="4.66667" fill="white"/>
            <rect y="30" width="9.33333" height="10" rx="4.66667" fill="white"/>
            <rect y="44.9999" width="9.33333" height="10" rx="4.66667" fill="white"/>
            <rect y="60.0001" width="9.33333" height="10" rx="4.66667" fill="white"/>
            <rect y="75" width="9.33333" height="10" rx="4.66667" fill="white"/>
            <rect x="18.6667" y="15.0002" width="9.33333" height="10" rx="4.66667" fill="white"/>
            <rect x="18.6667" y="30" width="9.33333" height="10" rx="4.66667" fill="white"/>
            <rect x="18.6667" y="44.9999" width="9.33333" height="10" rx="4.66667" fill="white"/>
            <rect x="18.6667" y="60.0001" width="9.33333" height="10" rx="4.66667" fill="white"/>
            <rect x="18.6667" y="75" width="9.33333" height="10" rx="4.66667" fill="white"/>
            <rect x="18.6667" y="89.9998" width="9.33333" height="10" rx="4.66667" fill="white"/>
        </svg>
    </div>
    <div class="center-container">
        <a href="/product">
            <button class="button">Shop now</button>
        </a>
    </div>


    


    <div class="point2">
        <svg xmlns="http://www.w3.org/2000/svg" width="28" height="100" viewBox="0 0 28 100" fill="none">
            <rect width="9.33333" height="10" rx="4.66667" fill="white"/>
            <rect y="15.0002" width="9.33333" height="10" rx="4.66667" fill="white"/>
            <rect y="30" width="9.33333" height="10" rx="4.66667" fill="white"/>
            <rect y="44.9999" width="9.33333" height="10" rx="4.66667" fill="white"/>
            <rect y="60.0001" width="9.33333" height="10" rx="4.66667" fill="white"/>
            <rect y="75" width="9.33333" height="10" rx="4.66667" fill="white"/>
            <rect x="18.6667" y="15.0002" width="9.33333" height="10" rx="4.66667" fill="white"/>
            <rect x="18.6667" y="30" width="9.33333" height="10" rx="4.66667" fill="white"/>
            <rect x="18.6667" y="44.9999" width="9.33333" height="10" rx="4.66667" fill="white"/>
            <rect x="18.6667" y="60.0001" width="9.33333" height="10" rx="4.66667" fill="white"/>
            <rect x="18.6667" y="75" width="9.33333" height="10" rx="4.66667" fill="white"/>
            <rect x="18.6667" y="89.9998" width="9.33333" height="10" rx="4.66667" fill="white"/>
        </svg>
    </div>

    <div class="circle">
        <img src="../components/protein.png" alt="Your Image">
    </div>




</template>

<style scoped>

.circle img {
  max-width: 100%;
  max-height: 100%;
  object-fit: cover;
  margin-top: 150px;
}
.circle {
  min-width: 200px;
  width: 548.453px;
  height: 549.005px;
  transform: rotate(0.5deg);
  flex-shrink: 0;
  border-radius: 50%;
  background: #FFB800;
  position: fixed;
  top: 20px;
  right: -150px;
  margin-top: 60px;
  display: flex;
  align-items: center;
  justify-content: center;
}



.point2 {
    width: 28px;
    height: 100px;
    transform: rotate(-90deg);
    flex-shrink: 0;
    position: fixed;
    top: 30px; 
    right: 700px; 
}


  .point {
    width: 28px;
    height: 100px;
    flex-shrink: 0;
    margin-left: 100px;
  }

  template {
    background: #222;
    display: flex;
    flex-direction: column;
    align-items: center; 
    justify-content: center; 
    margin: 0; 
  }

  .autumn, .high, .sale {
    transform: rotate(-10deg);
    font-style: normal;
    font-weight: bold; 
    margin: 0;
  }

  .autumn {
    color: #FFF;
    min-width: 601px;
    font-family: Gochi Hand;
    font-size: 40px;
    margin-left: 470px;
    margin-bottom: -25px;
    margin-top: 200px;
  }

  .high {
    color: #FFB800;
    font-family: Inter;
    font-size: 100px;
    margin-bottom: -20px;
    margin-left: 400px; 
  }

  .sale {
    color: #FFF;
    font-family: Inter;
    font-size: 80px;
    margin-left: 700px;
    margin-top: -40px; 
  }


.center-container {
  text-align: center;
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
}

.button:hover {
  background: #E5A500;
}

.button:active {
  background: #D39C00;
}

.center-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 30vh;
  margin: 0;
}



</style>
