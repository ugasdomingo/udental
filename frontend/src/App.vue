<script setup lang="ts">
// Import layout components
import HeaderComponent from './layout/HeaderComponent.vue';
import FooterComponent from './layout/FooterComponent.vue';
// Import other components
import HeroComponent from './components/HeroComponent.vue';
import ServicesComponent from './components/ServicesComponent.vue';
import SocialProofComponent from './components/SocialProofComponent.vue';
import ContactComponent from './components/ContactComponent.vue';
</script>

<template>
    <main>
        <HeaderComponent />
        <HeroComponent />
        <ServicesComponent />
        <SocialProofComponent />
        <ContactComponent />
        <FooterComponent />
    </main>
</template>

<style scoped lang="scss">
main {
    width: 100%;
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
}
</style>
