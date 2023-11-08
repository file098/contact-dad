<template>
    <div class="card">
        <div class="header">
            <div class="card-title">
                Oreste
                <br />
                Di Gennaro
            </div>
            <div class="card-subtitle">Guida ciclista</div>
        </div>
    </div>
    <div class="down-arrow" @click="scrollDown">
        <i class="fas fa-angle-down"></i>
    </div>
    <div class="description">
        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Nam praesentium
        tenetur et pariatur. Ipsum voluptatum quisquam labore ipsam
    </div>
    <button class="contact-me">Contattami</button>
    <!-- <iframe class="komoot-iframe" src="https://www.komoot.com/user/3227558101012/embed?stats=1" width="640" height="580" frameborder="0" scrolling="no"></iframe> -->
</template>

<script>
import "@fortawesome/fontawesome-free/css/all.css";
export default {
    name: "MainPage",
    methods: {
        scrollDown() {
            window.scrollTo({
                top: window.innerHeight,
                behavior: "smooth",
            });
        },
    },
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700&display=swap");

.card {
    position: relative;
    height: 80vh;
    display: flex;
    flex-direction: column;
    justify-content: end;

    color: #fff;
    background-image: linear-gradient(rgba(0, 0, 0, 0.3), rgba(0, 0, 0, 0.3)),
        url("/src/assets/card-bg.jpeg");
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center center;

    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.5);
    border-radius: 50px;

    .header {
        margin-top: 2rem;
        display: flex;
        flex-flow: column;
        text-align: start;
        margin: 2rem;

        .card-title {
            font: 500 48px Poppins;
            text-transform: uppercase;
        }

        .card-subtitle {
            font: 400 16px Poppins;
        }
    }
}

@keyframes bounce {

    0%,
    20%,
    50%,
    80% {
        transform: translateY(0);
    }

    40% {
        transform: translateY(-10px);
    }

    60% {
        transform: translateY(-5px);
    }

    100% {
        transform: translateY(0);
    }
}

.down-arrow {
    cursor: pointer;
    margin: 2rem 0 0.5rem 0;
    transform: scale(1.5);

    & i {
        animation: bounce 2s infinite;
    }
}

.description {
    font: 1rem Poppins;
    background-color: #fff;
    padding: 20px;
    text-align: start;
    margin: 1rem 0;
}

.komoot-iframe {
    padding: 1rem;
    border-radius: 10px;
    max-width: 90vw;
}

.contact-me {
    font: normal 24px Poppins, sans-serif;
    width: 50%;
    border-radius: 26px;
    padding: 20px;
    margin: 0 auto;
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.33);
    background: linear-gradient(180deg,
            rgba(142, 205, 60, 1) 0%,
            rgba(108, 171, 39, 1) 100%);
    color: white;
    border: none;
    cursor: pointer;
}</style>
