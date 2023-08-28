<script setup lang="ts"></script>

<template>
    <section class="services-container">
        <div class="services-content">
            <h2>Our Clinic Services</h2>
            <p class="subtitle">
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, voluptatum.
            </p>
        </div>
        <div class="services-cards-container">
            <div class="service">
                <img src="../assets/svg/tooth-clean.svg" alt="tooth-clean" />
                <h2>Tooth Whitening</h2>
                <p>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, voluptatum.
                </p>
            </div>
            <div class="service">
                <img src="../assets/svg/tooth-implant.svg" alt="tooth-implant" />
                <h2>Dental Implants</h2>
                <p>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, voluptatum.
                    Lorem ipsum dolor sit amet consectetur adipisicing.
                </p>
            </div>
            <div class="service">
                <img src="../assets/svg/tooth-exam.svg" alt="tooth-exam" />
                <h2>Oral Exam</h2>
                <p>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, voluptatum.
                    Lorem ipsum dolor sit amet consectetur.
                </p>
            </div>
            <div class="service">
                <img src="../assets/svg/tooth-medicine.svg" alt="tooth-medicine" />
                <h2>Proper Medicine</h2>
                <p>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, voluptatum.
                    Lorem, ipsum.
                </p>
            </div>
            <div class="service">
                <img src="../assets/svg/tooth-crack.svg" alt="tooth-crack" />
                <h2>Craked Thooth</h2>
                <p>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, voluptatum.
                    Lorem ipsum dolor sit amet.
                </p>
            </div>
            <div class="service">
                <img src="../assets/svg/tooth-protected.svg" alt="tooth-protected" />
                <h2>Tooth Protection</h2>
                <p>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, voluptatum.
                    Lorem, ipsum dolor.
                </p>
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
.services-container {
    display: flex;
    flex-direction: column;
    min-height: 90vh;
    width: 100%;
    box-sizing: border-box;
    padding: 4rem 0;

    .services-content {
        text-align: center;

        h2 {
            color: var(--color-primary);
            margin-bottom: 1rem;
        }

        .subtitle {
            color: var(--color-primary);
            text-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
            padding: 0 1rem;
        }
    }

    .services-cards-container {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        width: 100%;
        box-sizing: border-box;
        padding: 2rem;
        margin-top: 4rem;

        .service {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            width: 350px;
            max-height: 350px;
            box-sizing: border-box;
            padding: 2rem;
            margin: 1rem;
            background-color: #fff;
            border-radius: 1rem;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
            transition: all 0.5s ease-in-out;

            &:hover {
                transform: scale(1.1);
            }

            img {
                width: 5rem;
                height: 5rem;
                margin-bottom: 1rem;
            }

            h2 {
                font-size: 1.5rem;
                font-weight: 700;
                color: var(--color-primary);
                margin-bottom: 1rem;
            }

            p {
                font-size: 1rem;
                font-weight: 400;
                color: var(--color-primary);
            }
        }
    }
}

@media screen and (max-width: 768px) {
    .services-container {
        .services-cards-container {
            margin-top: 0;
            .service {
                width: 100%;
                max-height: 100%;
            }
        }
    }
}
</style>
