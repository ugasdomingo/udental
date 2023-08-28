<script setup lang="ts"></script>

<template>
    <section class="contact-container">
        <img src="../assets/image/hero.webp" alt="image" class="overload" />
        <h2>Contact us</h2>
        <p class="subtitle">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Nulla voluptate sunt molestiae.
        </p>
        <div class="contact-card-container">
            <div class="contact-card">
                <div class="contact-card-content">
                    <h3>Address</h3>
                    <p>
                        1234 Main Street
                        <br />
                        New York, NY 10001
                    </p>
                </div>
            </div>
            <div class="contact-card">
                <div class="contact-card-content">
                    <h3>Phone</h3>
                    <p>1-800-555-5555</p>
                </div>
            </div>
            <div class="contact-card">
                <div class="contact-card-content">
                    <h3>Email</h3>
                    <p>info@udentaladvison.com</p>
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
.contact-container {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 2rem 0;
    background-color: var(--color-primary);
    color: var(--color-white);
    box-sizing: border-box;
    position: relative;

    h2 {
        margin-bottom: 1rem;
    }

    .subtitle {
        margin-bottom: 2rem;
        padding: 0 1rem;
    }

    .contact-card-container {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        align-items: center;
        gap: 2rem;
        width: 100%;
        box-sizing: border-box;

        .contact-card {
            display: flex;
            justify-content: center;
            gap: 1rem;
            width: 300px;
            height: 150px;
            padding: 1rem;
            background-color: var(--color-white);
            box-shadow: 0 0 10px rgba(255, 255, 255, 0.2);
            box-sizing: border-box;
            border-radius: 0.5rem;

            .contact-card-content {
                display: flex;
                flex-direction: column;
                justify-content: space-around;
                align-items: center;
                gap: 1rem;
                padding: 1rem;
                box-sizing: border-box;

                h3 {
                    color: var(--color-primary);
                    margin: 1rem 0;
                }

                p {
                    color: var(--color-primary);
                    margin: 1rem 0;
                }
            }
        }
    }
}

.overload {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    object-fit: cover;
    opacity: 0.2;
}
</style>
