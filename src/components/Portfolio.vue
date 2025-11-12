<template>
    <div class="portfolio" id="about">
        <p class="portfolio__title">Lorem Ipsum is simply dummy text of the printing.</p>
        <p class="portfolio__subtitle">Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's</p>
        
        <div class="portfolio__contentSection portfolio__contentSection--1">
            <div class="portfolio__contentSection__text">
                <div class="portfolio__contentSection__text__container">
                    <Icon class="portfolio__contentSection__text__container--img1"/>
                    <div class="portfolio__contentSection__text__container__container2">
                        <p class="portfolio__contentSection__text__container-title">Lorem Ipsum is simply dummy text</p>
                        <p class="portfolio__contentSection__text__container-subtitle">Lorem Ipsum is simply dummy text</p>
                    </div>
                </div>
                <p class="portfolio__contentSection__text-title"><span class="highlight">Lorem Ipsum</span> is simply dummy text of the printing.</p>
                <p class="portfolio__contentSection__text-subtitle">KODEX TECHNOLOGY (PVT) LTD is a team of experienced mobile and web applications and website builders measuring dozens of completed projects. We build and develop mobile applications for several top platforms, including Android & IOS.</p>
            </div>
            <img class="portfolio__contentSection-img" :src="imgSrcImg1" alt="img1.jpg">
        </div>
        <div class="portfolio__contentSection portfolio__contentSection--2">
            <img class="portfolio__contentSection-img" :src="imgSrcImg2" alt="img2.png">
            <div class="portfolio__contentSection__text">
                <div class="portfolio__contentSection__text__container">
                    <Icon class="portfolio__contentSection__text__container--img2"/>
                    <div class="portfolio__contentSection__text__container__container2">
                        <p class="portfolio__contentSection__text__container-title">Lorem Ipsum is simply dummy text</p>
                        <p class="portfolio__contentSection__text__container-subtitle">Lorem Ipsum is simply dummy text</p>
                    </div>
                </div>
                <p class="portfolio__contentSection__text-title"><span class="highlight">Lorem Ipsum</span> is simply dummy text of the printing.</p>
                <p class="portfolio__contentSection__text-subtitle">KODEX TECHNOLOGY (PVT) LTD is a team of experienced mobile and web applications and website builders measuring dozens of completed projects. We build and develop mobile applications for several top platforms, including Android & IOS.</p>
            </div>
        </div>
        <div class="portfolio__contentSection portfolio__contentSection--3">
            <div class="portfolio__contentSection__text portfolio__contentSection__text3">
                <div class="portfolio__contentSection__text__container">
                    <Icon class="portfolio__contentSection__text__container--img3"/>
                    <div class="portfolio__contentSection__text__container__container2">
                        <p class="portfolio__contentSection__text__container-title">Lorem Ipsum is simply dummy text</p>
                        <p class="portfolio__contentSection__text__container-subtitle">Lorem Ipsum is simply dummy text</p>
                    </div>
                </div>
                <p class="portfolio__contentSection__text-title"><span class="highlight">Lorem Ipsum</span> is simply dummy text of the printing.</p>
                <p class="portfolio__contentSection__text-subtitle">KODEX TECHNOLOGY (PVT) LTD is a team of experienced mobile and web applications and website builders measuring dozens of completed projects. We build and develop mobile applications for several top platforms, including Android & IOS.</p>
            </div>
            <img class="portfolio__contentSection-img portfolio__contentSection-img3" :src="imgSrcImg3" alt="img3.png">
        </div>
        <div class="portfolio__cards" id="blog">
            <div class="portfolio__cards__card portfolio__cards__card1">
                <p class="portfolio__card-title">Lorem Ipsum is simply dummy text.</p>
                <p class="portfolio__card-description">KODEX TECHNOLOGY (PVT) LTD is a team of experienced mobile and web applications and website builders measuring dozens of completed projects. We build and develop mobile applications for several top platforms, including Android & IOS.</p>
                <button class="portfolio__card-btn portfolio__card1-btn">View More</button>
            </div>
            <div class="portfolio__cards__card portfolio__cards__card2">
                <p class="portfolio__card-title">Lorem Ipsum is simply dummy text.</p>
                <p class="portfolio__card-description">KODEX TECHNOLOGY (PVT) LTD is a team of experienced mobile and web applications and website builders measuring dozens of completed projects. We build and develop mobile applications for several top platforms, including Android & IOS.</p>
                <button class="portfolio__card-btn portfolio__card2-btn">View More</button>
            </div>
        </div>
        <div class="portfolio__partners">
            <img class="portfolio__partners-img" :src="imgSrcBeneoshop" />
            <img class="portfolio__partners-img" :src="imgSrcCaspio" />
            <img class="portfolio__partners-img" :src="imgSrcHypergrid" />
            <img class="portfolio__partners-img" :src="imgSrcLeotrippi" />
        </div>
    </div>
</template>

<script setup>
import imgSrcImg1 from '@/assets/img1.jpg'
import imgSrcImg2 from '@/assets/img2.png'
import imgSrcImg3 from '@/assets/img3.png'
import imgSrcBeneoshop from '@/assets/beneoshop.png'
import imgSrcCaspio from '@/assets/caspio.png'
import imgSrcHypergrid from '@/assets/hypergrid.png'
import imgSrcLeotrippi from '@/assets/leotrippi.png'
import Icon from '@/components/Icon.vue';
</script>

<style>
.portfolio{
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 70px 20px;
    gap: 30px;
    position: relative;
    overflow: hidden;
}

.portfolio__title{
    font-weight: 600;
    font-size: 33px;
    line-height: 160%;
    color: #252525;
    text-align: center;
}

.portfolio__subtitle{
    font-weight: 400;
    font-size: 18px;
    line-height: 175%;
    color: #868686;
    width: 50%;
    text-align: center;
}

.portfolio__contentSection{
    display: flex;
    justify-content: center;
    width: 100%;
    align-items: center;
}

.portfolio__contentSection__text{
    width: 40%;
}

.portfolio__contentSection-img{
    width: 50%;
    overflow: hidden;
}

.portfolio__contentSection-img3{
    width: 60%;
    position: relative;
    left: -10%;
}

.portfolio__contentSection__text3{
    position: relative;
    left: 5%;
}

.portfolio__contentSection__text__container{
    display: flex;
    align-items: center;
    gap: 15px;
}

.portfolio__contentSection__text__container-title{
    font-weight: 500;
    font-size: 17px;
    line-height: 129%;
}

.portfolio__contentSection__text__container-subtitle{
    font-weight: 400;
    font-size: 14px;
    line-height: 175%;
    color: #868686;
}

.portfolio__contentSection__text__container--img{
    padding: 10px;
    border-radius: 100%;
    width: 30px;
    height: 30px;
    flex-shrink: 0;
}

.portfolio__contentSection__text__container--img1{
    background-color: #08D3BB;
}
.portfolio__contentSection__text__container--img2{
    background-color: #1090CB;
}
.portfolio__contentSection__text__container--img3{
    background-color: #9208D3;
}

.portfolio__contentSection__text{
    display: flex;
    flex-direction: column;
    gap: 40px;
}

.portfolio__contentSection__text-title{
    font-weight: 500;
    font-size: 30px;
    line-height: 170%;
}

.portfolio__contentSection__text-subtitle{
    font-weight: 400;
    font-size: 16px;
    line-height: 170%;
    color: #545454;
}

.highlight {
    color: #1090CB;
}

.portfolio__contentSection--1::after{
    content: "";
    position: absolute;
    width: 497px;
    height: 505px;
    right: -200px;
    border-radius: 50%;
    background: radial-gradient(50% 50% at 50% 50%, #DED9FF 0%, rgba(196, 196, 196, 0) 100%);
    z-index: 1;
}
.portfolio__contentSection--2::after{
    content: "";
    position: absolute;
    width: 497px;
    height: 505px;
    left: -200px;
    border-radius: 50%;
    background: radial-gradient(50% 50% at 50% 50%, #F3FFD9 0%, rgba(196, 196, 196, 0) 100%);
    z-index: -1;
}
.portfolio__contentSection--3::after{
    content: "";
    position: absolute;
    width: 497px;
    height: 505px;
    right: -200px;
    border-radius: 50%;
    background: radial-gradient(50% 50% at 50% 50%, #DED9FF 0%, rgba(196, 196, 196, 0) 100%);
    z-index: -1;
}

.portfolio__cards {
    position: relative;
    display: flex;
    width: 100%;
    justify-content: center;
    align-items: flex-start;
    gap: 50px;
    padding: 60px;
    overflow: hidden;
}

.portfolio__cards::after {
    content: "";
    position: absolute;
    bottom: -10px;
    right: -100px;
    width: 300px;
    height: 300px;
    background: radial-gradient(50% 50% at 50% 50%, #FFD9EB 0%, rgba(255, 255, 255, 0) 100%);
    border-radius: 50%;
    z-index: -1;
}

.portfolio__cards__card {
    position: relative;
    width: 40%;
    padding: 40px 30px;
    border-radius: 20px;
    text-align: center;
    box-shadow: 0 5px 20px rgba(0,0,0,0.05);
    transition: all 0.3s ease;
}

.portfolio__cards__card1 {
    background-color: #F4F4F4;
}

.portfolio__cards__card2 {
    background-color: #1090CB;
    color: white;
}

.portfolio__card-title {
    font-weight: 600;
    font-size: 25px;
    margin-bottom: 20px;
}

.portfolio__card-description {
    font-size: 16px;
    font-weight: 400;
    line-height: 170%;
    margin-bottom: 30px;
}

.portfolio__card-btn {
    padding: 10px 25px;
    border: none;
    border-radius: 6px;
    font-weight: 500;
    cursor: pointer;
    transition: all 0.3s ease;
}

.portfolio__card1-btn {
    background-color: #1090CB;
    color: #fff;
}

.portfolio__card2-btn {
    background-color: #fff;
    color: #1090CB;
}

.portfolio__card1-btn:hover {
    opacity: 0.85;
}

.portfolio__card2-btn:hover {
    background-color: #f0f0f0;
}

.portfolio__card-btn:active{
    transform: scale(0.95);
}

.portfolio__cards__card2::after {
    content: "";
    position: absolute;
    top: -35px;
    right: 10px;
    width: 70px;
    height: 70px;
    transform: rotate(20.37deg);
    background: url("../assets/bell.png") no-repeat center/contain;
}

.portfolio__text{
    font-weight: 500;
    font-size: 24px;
}

.portfolio__partners{
    display: flex;
    justify-content: center;
    width: 100%;
    gap: 10%;
}

.portfolio__partners-img{
    width: 15%;
}

.portfolio__partners::after {
    content: "";
    position: absolute;
    bottom: 0px;
    left: -200px;
    width: 500px;
    height: 500px;
    background: radial-gradient(50% 50% at 50% 50%, #FAFFD9 0%, rgba(255, 255, 255, 0) 100%);
    border-radius: 50%;
    z-index: -1;
}

@media (max-width: 768px) {
    .portfolio__cards {
        flex-direction: column;
        align-items: center;
    }

    .portfolio__cards__card {
        width: 80%;
    }
}


@media (max-width: 850px) {

    .portfolio__contentSection--3{
        padding-right: 10%;
    }

    .portfolio__contentSection{
        flex-direction: column;
        width: 100%;
        margin-top: 50px;
    }

    .portfolio__subtitle{
        width: 80%;
    }

    .portfolio__contentSection__text{
        width: 80%;
        display: flex;
        justify-content: center;
        text-align: center;
    }

    .portfolio__contentSection__text__container{
        justify-content: center;
    }

    .portfolio__contentSection__text__container-title{
        font-size: 15px;
    }

    .portfolio__contentSection__text__container-subtitle{
        font-size: 12px;
    }

    .portfolio__contentSection--2{
        flex-direction: column-reverse;
    }

    .portfolio__contentSection-img{
        width: 70%;
    }
    .portfolio__contentSection-img3{
        width: 90%;
    }

    .portfolio__contentSection--1::after{
        width: 300px;
        height: 300px;
        right: -100px;
        top: 800px;
    }
    .portfolio__contentSection--2::after{
        width: 300px;
        height: 300px;
        left: -100px;
        top: 1600px;
    }
    .portfolio__contentSection--3::after{
        width: 300px;
        height: 300px;
        right: -100px;
        top: 2400px;
    }
}

@media (max-width: 500px) {
    .portfolio__title{
        font-size: 25px;
    }

    .portfolio__subtitle{
        width: 80%;
        font-size: 15px;
    }

    .portfolio__contentSection__text{
        width: 100%;
    }

    .portfolio__contentSection__text__container{
        width: 100%;
    }

    .portfolio__contentSection__text-title{
        font-size: 20px;
    }

    .portfolio__contentSection__text-subtitle{
        font-size: 12px;
    }

    .portfolio__card-title{
        font-size: 20px;
    }

    .portfolio__card-description{
        font-size: 13px;
    }

    .portfolio__contentSection--1::after{
        top: 700px;
    }
    .portfolio__contentSection--2::after{
        top: 1300px;
    }
    .portfolio__contentSection--3::after{
        top: 1950px;
    }

    .portfolio__text{
        font-size: 17px;
    }

}
@media (max-width: 380px) {
    .portfolio__contentSection--1::after{
        top: 700px;
    }
    .portfolio__contentSection--2::after{
        top: 1200px;
    }
    .portfolio__contentSection--3::after{
        top: 1750px;
    }

    .portfolio__contentSection__text__container__container2 {
        max-width: 90%;
    }

    .portfolio__contentSection__text__container-title {
        font-size: 14px;
    }

    .portfolio__contentSection__text__container-subtitle {
        font-size: 12px;
    }
}

</style>
