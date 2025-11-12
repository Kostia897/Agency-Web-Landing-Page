<template>
    <header class="header">
        <div class="header__logo">
            <p>LOGO</p>
        </div>

        <nav class="header__nav">
            <a href="#home" class="header__nav-link header__nav-link--home">Home</a>
            <a href="#about"class="header__nav-link">About us</a>
            <a href="#services" class="header__nav-link">Services</a>
            <a href="#blog" class="header__nav-link">Blog</a>
        </nav>

        <button class="header__btn">Contact us</button>
    </header>
</template>

<style>
.header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 30px;
    background-color: #ffffff;
    border-bottom: 1px solid #C4C4C4;
    gap: 50px;
    white-space: nowrap;
    font-size: 20px;
    height: 50px;
}

.header__logo {
    width: 50%;
}

.header__logo p {
    color: #1090CB;
    font-weight: 700;
    font-size: 29px;
}

.header__nav {
    display: flex;
    gap: 50px;
    justify-content: space-between;
    align-items: center;
}

.header__nav-link {
    text-decoration: none;
    color: #000000;
    position: relative;
    font-weight: 400;
    font-size: 16px;
}

.header__nav-link:hover{
    text-decoration: underline;
    cursor: pointer;
}

.header__nav-link--home {
    text-decoration: underline;
    text-decoration-thickness: 1px;
    text-underline-offset: 2px;
    color: #1090CB;
}

.header__btn {
    padding: 10px 20px;
    background-color: #1090CB;
    color: #fff;
    border: none;
    cursor: pointer;
    transition: all 0.3s ease;
    border-radius: 6px;
    font-size: 13px;
    font-weight: 400;
}

.header__btn:hover {
    opacity: 0.8;
}

.header__btn:active {
    transform: scale(0.95);
}

@media (max-width: 800px) {
    .header {
        gap: 20px;
        padding: 10px;
        font-size: 15px;
    }
    .header__nav {
        gap: 20px;
    }
    .header__btn {
        padding: 7px 10px;
    }
    .header__logo {
        font-size: 10px;
    }
}

@media (max-width: 500px) {
    .header {
        gap: 10px;
        padding: 10px;
        font-size: 13px;
    }
    .header__nav {
        gap: 6px;
        font-size: 10px;
    }
    .header__btn {
        padding: 5px;
        font-size: 11px;
    }
    .header__logo {
        font-size: 8px;
    }
    .header__logo p {
        font-size: 20px;    
    }
    .header__nav-link {
        font-size: 10px;
    }
}
</style>
