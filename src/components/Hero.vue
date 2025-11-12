<template>
    <div class="hero">
        <div class="hero__content" id="home">
            <h1 class="hero__title">
                Experienced <span class="highlight">mobile and web</span><br />
                applications and website<br />
                builders measuring.
            </h1>

            <p class="hero__text">
                KODEX TECHNOLOGY (PVT) LTD is a team of experienced mobile and web applications and website builders measuring dozens of completed projects. We build and develop mobile applications for several top platforms, including Android  & IOS.
            </p>

            <div class="hero__buttons">
                <button class="hero__btn hero__btn--primary">Contact us</button>
                <button class="hero__btn hero__btn--secondary">View more</button>
            </div>
        </div>

        <div class="hero__images">
            <div class="hero__images--circle"></div>
            <img :src="imgSrcSucclent" alt="succlent-angle.png" class="hero__image hero__image--succlent">
            <img :src="imgSrcPlant" alt="big-plant.png" class="hero__image hero__image--plant">
            <img :src="imgSrcCuboid" alt="cuboid.png" class="hero__image hero__image--cuboid">
            <img :src="imgSrcBill" alt="bill-sitting-using-laptop.png" class="hero__image hero__image--bill">
        </div>
        <svg class="hero__shape hero__shape--right" width="47" height="531" viewBox="0 0 47 531" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M16.7283 186.353C40.6069 228.272 19.7551 282.23 45.6957 347.368C53.0404 365.811 56.5381 376.626 66.8342 393.597C116.83 476.003 189.595 521.937 285.656 529.148C352.27 534.148 431.191 533.543 460.244 467.249C489.603 400.257 473.972 315.214 423.839 241.2C368.644 159.713 320.481 102.416 231.244 45.3169C183.487 14.7592 88.0571 -27.7495 33.1692 24.9451C-8.61798 65.0625 -7.15036 144.434 16.7283 186.353Z" fill="#1090CB"/>
        </svg>
        <svg class="hero__shape hero__shape--left" width="55" height="609" viewBox="0 0 55 609" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M-391.591 0.0580718C-445.452 -1.66818 -477.316 35.2762 -501.572 83.3967C-545.833 171.201 -560.967 276.157 -546.418 365.515C-531.868 454.873 -479.047 516.999 -426.364 554.226C-346.508 610.655 -325.59 612.264 -247.5 606.682C-190.503 602.607 -159.808 595.228 -93.8058 561.507C-27.8039 527.786 76.4386 464.776 50.4221 374.21C29.8276 302.518 -112.879 281.976 -112.879 281.976C-112.879 281.976 -179.389 274.376 -219.359 243.412C-260.729 211.364 -286.937 127.7 -286.937 127.7C-286.937 127.7 -327.164 2.12298 -391.591 0.0580718Z" fill="#08D3BB"/>
        </svg>
    </div>

</template>

<script setup>
import imgSrcSucclent from '@/assets/succlent-angle.png'
import imgSrcPlant from '@/assets/big-plant.png'
import imgSrcCuboid from '@/assets/cuboid.png'
import imgSrcBill from '@/assets/bill-sitting-using-laptop.png'
</script>

<style>
.hero {
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    background: #1090CB1A;
}

.hero__content {
    width: 50%;
    padding: 100px 50px;
}

.hero__title {
    font-size: 40px;
    font-weight: 600;
    color: #000;
    margin-bottom: 20px;
    line-height: 1.3;
}

.highlight {
    color: #1090CB;
}

.hero__text {
    color: #5C5C5C;
    font-size: 16px;
    line-height: 2;
    margin-bottom: 40px;
    font-weight: 400;
}

.hero__buttons {
    display: flex;
    gap: 20px;
}

.hero__btn {
    padding: 12px 30px;
    border-radius: 8px;
    font-weight: 400;
    cursor: pointer;
    transition: all 0.3s ease;
    font-size: 16px;
}

.hero__btn--primary {
    background-color: #1090CB;
    color: #fff;
    border: none;
}

.hero__btn--primary:hover {
    opacity: 0.85;
}

.hero__btn--primary:active {
    transform: scale(0.95);
}

.hero__btn--secondary {
    background-color: transparent;
    border: 1px solid #1090CB;
    color: #1090CB;
    background-color: white;
}

.hero__btn--secondary:hover {
    background-color: #1090CB;
    color: #fff;
}

.hero__btn--secondary:active {
    transform: scale(0.95);
}

.hero__images {
    width: 40%;
    height: 100%;
    position: relative;
    pointer-events: none;
}

.hero__image{
    position: absolute;
}

.hero__image--succlent{
    height: 66px;
    left: 55px;
    top: -200px;
}

.hero__image--plant{
    height: 185px;
    left: 260px;
    top: 52px;
}

.hero__image--cuboid{
    height: 68px;
    transform: rotate(57.89deg);
    left: 345px;
    top: -220px;
}

.hero__image--bill{
    height: 763px;
    top: -480px;
    left: -85px;
}

.hero__shape{
    position: absolute;
}

.hero__shape--right{
    right: 0;
    top: 200px;
}

.hero__shape--left{
    left: -20px;
    top: 200px;
}

.hero__images--circle{
    position: absolute;
    top: -360px;
    left: 50px;
    width: 400px;
    height: 400px;
    border-radius: 500px;
    background: radial-gradient(50% 50% at 50% 50%, #FDFFEA 0%, rgba(196, 196, 196, 0) 100%);
}

@media (max-width: 1170px) {
    .hero__content{
        width: 40%;
    }

    .hero__images{
        width: 50%;
    }
}

@media (max-width: 940px) {
    .hero__content{
        width: 35%;
    }

    .hero__images{
        width: 58%;
    }
}

@media (max-width: 850px) {
    .hero {
        flex-direction: column;
        text-align: center;
    }

    .hero__content{
        width: 70%;
    }

    .hero__images{
        display: none;
    }

    .hero__title {
        font-size: 32px;
    }

    .hero__buttons{
        display: flex;
        justify-content: center;
        gap: 20px;
        white-space: nowrap;
    }
}

@media (max-width: 500px) {
    .hero__title{
        font-size: 22px;
    }  
    .hero__text{
        font-size: 13px;
    }  
    .hero__btn {
        font-size: 12px;
    }
    .hero__shape--left{
        top: 150px;
    }
}

@media (max-width: 380px) {
    .hero__buttons{
        gap: 5px;
    }

    .hero__shape--left{
        left: -25px;
        top: 200px;
    }   
}
</style>
