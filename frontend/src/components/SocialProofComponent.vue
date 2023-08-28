<script setup lang="ts"></script>

<template>
    <section class="social-container">
        <h2>What our patients say</h2>
        <p class="subtitle">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Nulla voluptate sunt molestiae.
        </p>
        <div class="social-card-container">
            <div class="social-card">
                <div class="social-card-content">
                    <h3>Samantha</h3>
                    <p>
                        "Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam,
                        voluptatum. Lorem ipsum dolor sit amet consectetur adipisicing elit.
                        Quisquam, voluptatum."
                    </p>
                </div>
            </div>
            <div class="social-card">
                <div class="social-card-content">
                    <h3>Benjamin</h3>
                    <p>
                        "Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam,
                        voluptatum. Lorem ipsum dolor sit amet consectetur adipisicing elit.
                        Quisquam, voluptatum."
                    </p>
                </div>
            </div>
            <div class="social-card">
                <div class="social-card-content">
                    <h3>John Doe</h3>
                    <p>
                        "Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam,
                        voluptatum. Lorem ipsum dolor sit amet consectetur adipisicing elit.
                        Quisquam, voluptatum."
                    </p>
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
.social-container {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 2rem 0;
    background-color: #f5f5f5;
    box-sizing: border-box;

    h2 {
        color: var(--color-primary);
        margin-bottom: 1rem;
        text-align: center;
    }

    .subtitle {
        color: var(--color-primary);
        text-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
        margin-bottom: 2rem;
        padding: 0 1rem;
    }

    .social-card-container {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        align-items: center;
        gap: 2rem;
        width: 100%;
        box-sizing: border-box;

        .social-card {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            width: 350px;
            max-height: 500px;
            border-radius: 1rem;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
            overflow: hidden;

            .social-card-content {
                display: flex;
                flex-direction: column;
                justify-content: center;
                align-items: center;
                padding: 2rem;
                box-sizing: border-box;

                h3 {
                    font-size: 2rem;
                    font-weight: 700;
                    margin-bottom: 1rem;
                }

                p {
                    font-size: 1rem;
                    text-align: center;
                }
            }
        }
    }
}

@media screen and (max-width: 768px) {
    .social-container {
        .social-card-container {
            .social-card {
                width: 100%;
            }
        }
    }
}
</style>
