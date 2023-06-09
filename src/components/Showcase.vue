<script setup lang="ts">
import { RouterLink } from 'vue-router';
</script>

<template>
    <div class="showcase">
        <div>
            <h1 class="gradient-text">Your Software Development Partner for Good</h1>
            <p>
                SolidFly builds dedicated teams and software solutions that create an impact – for your business and the world. Leverage our European tech expertise and Nordic business values to scale up and innovate.
            </p>
            <br><br>
            <RouterLink to="/about" class="button1">Let's Develop</RouterLink>
        </div>
        <div>
            <img alt="showcase" class="logo" src="@/assets/showcase-img.svg"  />
        </div>
    </div>
</template>
<style lang="scss">
.showcase {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap-reverse;
    height: 100vh;
    padding: 0 7%;

    div {
        width: 48%;
        margin: 1%;

        img {
            width: 100%;
        }

        h1 {
         font-family: 'Bagel Fat One', cursive;
         font-weight: bold;
         font-size: calc(10px + 4.5vmin);
        }
        p {
            font-family: 'DM Sans', sans-serif;
            margin-top: 1vh;
            font-size: calc(10px + 0.8vmin);
            color: var(--var-color-white);
        }
      
    }
}
</style>