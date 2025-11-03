<template>
    <form class="contactForm" @submit.prevent="Submit()">
        <p class="contactForm__text">Lorem Ipsum is simply dummy text of the printing.</p>
        <div class="contactForm__container">
            <input type="email" v-model="email" class="contactForm__container--input" placeholder="Enter your email">
            <input type="submit" class="contactForm__container--btn" value="SUBSCRIBE">
        </div>
    </form>
</template>

<script>
export default {
    data() {
        return {
            email: ''
        }
    },
    methods: {
        Submit() {
            console.log(this.email);
        }
    }
};
</script>

<style>
.contactForm{
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

.contactForm__text{
    font-weight: 600;
    font-size: 30px;
    line-height: 170%;
    width: 50%;
    text-align: center;
}

.contactForm__container{
    display: flex;
    width: 100%;
    justify-content: center;
    gap: 20px;
}

.contactForm__container--input{
    padding: 20px 30px;
    width: 40%;
    color: #787878;
    background-color: white;
    border: none;
    border-radius: 10px;
    font-weight: 400;
    font-size: 16px;
}

.contactForm__container--btn{
    padding: 10px 40px;
    color: white;
    font-weight: 500;
    font-size: 16px;
    border-radius: 10px;
    border: none;
    background-color: black;
    transition: all 0.3s ease;
}

.contactForm__container--btn:hover{
    opacity: 0.75;
}

.contactForm__container--btn:active{
    transform: scale(0.95);    
}

.contactForm::after {
    content: "";
    position: absolute;
    top: -35px;
    left: 10%;
    width: 66px;
    height: 66px;
    transform: rotate(-24.8deg);
    background: url("../assets/star.png") no-repeat center/contain;
}

.contactForm::before {
    content: "";
    position: absolute;
    top: 50px;
    right: 20%;
    width: 54px;
    height: 54px;
    transform: rotate(-24.8deg);
    background: url("../assets/pai chart.png") no-repeat center/contain;
}


@media (max-width: 500px) {
    .contactForm__container{
        flex-direction: column;
        align-items: center;
    }

    .contactForm__container--btn{
        width: min-content;
    }

    .contactForm__text{
        font-size: 20px;
        width: 70%;
    }
}
</style>
