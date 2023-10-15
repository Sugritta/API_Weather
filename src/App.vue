<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header class="d-flex flex-wrap justify-content-center py-3" style="width: 100%;  background-color: rgba(255, 255, 255, 0.8);">
        <RouterLink to="/" class="d-flex align-items-center mb-3 mb-md-0 me-md-auto link-body-emphasis text-decoration-none">
        <svg class="bi me-2" width="50" height="70"></svg>
        <span class="fs-3" style="color: rgb(20, 46, 127); " ><h2>WeatherDay</h2></span>
        </RouterLink>
        <ul class="nav col-12 col-lg-auto my-2 justify-content-center my-md-0 text-small ">
            <li>
              <RouterLink to="/weather" class="nav-link text-white" style="color: rgb(13, 47, 72);"> 
                  <img class="bi d-block mx-auto mb-1" src="@/assets/cloud.png" alt="cart" width="24" height="24" >
                  <p style="color:rgb(11, 24, 88) ;">ข้อมูล</p>
              </RouterLink>
            </li>
        </ul>
    </header>

    <div class="mainbd">
      <RouterView />
    </div>
    
    
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=K2D:wght@400;500;600&display=swap');

body{
    background: linear-gradient(338deg, rgb(248, 189, 235) 0%, rgb(82, 114, 242) 100%);
    font-family: 'K2D', sans-serif;
}

p {
  margin: 0%;
}
</style>

