<script setup lang="ts"></script>

<template>
    <header>
        <img src="../assets/image/logo.webp" alt="Udental logo" />
        <div class="navegation">
            <a href="#services">Services</a>
            <a href="#about">About</a>
            <a href="#contact">Contact</a>
        </div>
    </header>
</template>

<style scoped lang="scss">
header {
    display: flex;
    justify-content: end;
    align-items: center;
    height: 10vh;
    padding: 0 3em;
    position: relative;

    img {
        width: 150px;
        object-fit: contain;
        position: absolute;
        top: 0;
        left: 3rem;
        z-index: 10;
    }
}
.navegation {
    display: flex;
    justify-content: end;
    align-items: center;
    width: 100%;
    height: 100%;
    gap: 1rem;

    a {
        text-decoration: none;
        color: #646cff;
        font-size: 1.25rem;
        font-weight: 400;
        padding: 0.5em;
        will-change: filter;
        transition: filter 300ms;
    }

    a:hover {
        filter: drop-shadow(0 0 2em var(--color-primary));
        background-color: var(--color-primary);
        color: var(--color-white);
        border-radius: 1rem;
    }
}

@media (max-width: 768px) {
    header {
        padding: 0;

        img {
            top: 0;
            left: 0;
            width: 100px;
        }
    }

    .navegation {
        gap: 0.5rem;
    }
}
</style>
