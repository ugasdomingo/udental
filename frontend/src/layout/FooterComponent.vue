<script setup lang="ts"></script>

<template>
    <footer>
        <h4>Udental Advisor</h4>
        <p>All right reserved</p>
    </footer>
    <!-- //Sticky Call button -->
    <a href="tel:" class="call-button">
        <i class="fas fa-phone-alt"></i>
    </a>
</template>

<style scoped lang="scss">
footer {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100%;
    max-height: 2.5rem;
    padding: 0 3rem;
    background-color: var(--color-primary);
    color: var(--color-white);
    font-size: 1.5em;
    font-weight: bold;
    padding: 0.5em;
    will-change: filter;
    transition: filter 300ms;

    h4 {
        margin: 0;
        font-size: 1.5rem;
    }

    p {
        margin: 0 0 0 1rem;
        padding: 0;
        opacity: 0.75;
    }
}

footer:hover {
    filter: drop-shadow(0 0 2em #646cffaa);
}

.call-button {
    position: fixed;
    bottom: 1rem;
    right: 1rem;
    width: 4rem;
    height: 4rem;
    border-radius: 50%;
    background-color: var(--color-primary);
    color: var(--color-white);
    font-size: 1.25rem;
    display: flex;
    justify-content: center;
    align-items: center;
    will-change: filter;
    transition: filter 300ms;
}
</style>
