<template>
    <form class="form" @submit.prevent="submit()" :style="{
                '--after-bg': `url(${imgSrcStar})`, 
                '--before-bg': `url(${imgSrcPaiChart})`
            }">
        <p class="form__text">Lorem Ipsum is simply dummy text of the printing.</p>
        <div class="form__container">
            <input type="email" v-model="email" class="form__input" placeholder="Enter your email">
            <button type="submit" class="form__btn">Subscribe</button>
        </div>
    </form>
</template>

<script>
import imgSrcStar from '@/assets/star.png'
import imgSrcPaiChart from '@/assets/pai-chart.png'
export default {
    data() {
        return {
            email: '',
            imgSrcStar,
            imgSrcPaiChart
        }
    },
    methods: {
        submit() {
            console.log(this.email);
        }
    }
};
</script>

<style>
.form{
    position: relative;
    width: 100%;
    background-color: #E8F4FA;
    display: flex;
    flex-direction: column;
    align-items: center;
    padding-top: 120px;
    padding-bottom: 120px;
    gap: 60px;
}

.form__text{
    font-weight: 600;
    font-size: 30px;
    line-height: 170%;
    width: 50%;
    text-align: center;
}

.form__container{
    display: flex;
    width: 100%;
    justify-content: center;
    gap: 20px;
}

.form__input{
    padding: 20px 30px;
    width: 40%;
    color: #787878;
    background-color: white;
    border: none;
    border-radius: 10px;
    font-weight: 400;
    font-size: 16px;
}

.form__btn{
    padding: 10px 40px;
    color: white;
    font-weight: 500;
    font-size: 16px;
    border-radius: 10px;
    border: none;
    background-color: black;
    transition: all 0.3s ease;
}

.form__btn:hover{
    opacity: 0.75;
}

.form__btn:active{
    transform: scale(0.95);    
}

.form::after, .form::before {
    content: "";
    position: absolute;
    background-repeat: no-repeat;
    background-position: center;
    background-size: contain;
}

.form::after {
    top: -35px;
    left: 10%;
    width: 66px;
    height: 66px;
    transform: rotate(-24.8deg);
    background-image: var(--after-bg);
}

.form::before {
    top: 50px;
    right: 20%;
    width: 54px;
    height: 54px;
    transform: rotate(-24.8deg);
    background-image: var(--before-bg);
}


@media (max-width: 500px) {
    .form__container{
        flex-direction: column;
        align-items: center;
    }

    .form__btn{
        width: min-content;
    }

    .form__text{
        font-size: 20px;
        width: 70%;
    }
}
</style>
