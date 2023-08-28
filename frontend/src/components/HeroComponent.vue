<script setup lang="ts"></script>

<template>
    <section class="hero-container">
        <img src="../assets/image/hero2.webp" alt="Hero Image" class="hero-image" />
        <div class="hero-content">
            <h1>Dental Services That<br />You Can Trust</h1>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ad, nulla.</p>
        </div>
    </section>
</template>

<style scoped lang="scss">
.hero-container {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 90vh;
    width: 100%;
    box-sizing: border-box;
    overflow: hidden;
    background-color: var(--color-white);
    position: relative;

    .hero-image {
        width: 100%;
        height: 100%;
        object-fit: cover;
        position: absolute;
        top: 0;
        left: 0;
    }

    .hero-content {
        position: absolute;
        top: 50%;
        left: 0;
        transform: translate(7%, -50%);
        text-align: center;
        background-color: var(--color-primary-transparent);
        border-radius: 1rem;
        padding: 2rem;
        box-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
        animation: slide 1.5s;

        h1 {
            font-size: 3rem;
            font-weight: 700;
            color: #fff;
            text-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
            margin-bottom: 1rem;
        }

        p {
            font-size: 1.5rem;
            font-weight: 400;
            color: #fff;
            text-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
        }
    }
}

@keyframes slide {
    0% {
        transform: translate(-10%, -50%) scale(0.5);
    }
    100% {
        transform: translate(10%, -50%) scale(1);
    }
}

@media screen and (max-width: 768px) {
    .hero-image {
        object-position: right;
    }

    @keyframes slide {
        0% {
            transform: translate(0, 0%) scale(0.5);
        }
        100% {
            transform: translate(7%, -50%) scale(1);
        }
    }
}
</style>
