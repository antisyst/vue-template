<script setup lang="ts">

</script>
<template>
    <div class="static_section">
        <div>
            <img src="@/icons/com.svg" alt="">
            <h1 class="gradient-text">Top 1%</h1>
            <p>of software development companies on Clutch</p>
        </div>
        <div>
            <img src="@/icons/top.svg" alt="">
            <h1 class="gradient-text">60%</h1>
            <p>of business is based on customer referrals</p>
        </div>
        <div>
            <img src="@/icons/nature.svg" alt="">
            <h1 class="gradient-text">CO2-Neutral</h1>
            <p>offsetting unavoidable emissions by reforestation</p>
        </div>
        <div>
            <img src="@/icons/security.svg" alt="">
            <h1 class="gradient-text">ISO 27001</h1>
            <p>data security certification by Bureau Veritas</p>
        </div>
    </div>
</template>
<style lang="scss">
    .static_section {
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: center;
        flex-wrap: wrap;
        padding: 10px 7%;
        text-align: center;
        margin-top: 10vh;
        margin-bottom: 9vh;

        div {
            width: 300px;
            height: 280px;
            margin: 20px 26px;
            color: var(--var-color-white);
            display: flex;
            flex-direction: column;
            align-items: flex-start;
            justify-content: center;
            
            img {
                width: 140px;
                filter: drop-shadow(0 0 0.65rem var(--var-color-prim));
            }
            h1 {
                font-family: 'Bagel Fat One', cursive;
                margin: 12px 0;
                font-size: calc(10px + 2.7vmin);
            }
            p {
                font-family: 'DM Sans', sans-serif;
                text-align: left;
                padding-right: 20px;
                font-size: 18px;
            }
        }
    }
</style>