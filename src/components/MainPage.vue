<template>
    <div class="card">
        <div class="header">
            <div class="card-title">
                Oreste
                <br>
                Di Gennaro
            </div>
            <div class="card-subtitle">
                Guida ciclista
            </div>
        </div>
        <div class="subcard">
            <div class="subcard-text">
                Lorem ipsum dolor sit, amet consectetur adipisicing elit. Nam
                praesentium tenetur et pariatur. Ipsum voluptatum quisquam labore ipsam
                sunt vel sed illo dolor optio ratione officiis voluptas mollitia, dolore
                eos.
            </div>
            <button class="contact-me">Contattami</button>
        </div>
    </div>
</template>

<script>
export default {
    name: "MainPage",
};
</script>

<style>
.card {
    height: 98vh;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
}

.header {
    margin-top: 2rem;
    display: flex;
    flex-flow: column;
}

.card-title {
    font-size: 2.5rem;
    font-weight: 400;
    text-transform: uppercase;
}

.subcard {
    position: relative;
    height: 70%;
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    align-items: center;
    margin: 0 2px;
    box-shadow: 0 0 10px rgba(63, 63, 63, 0.1);
    border-radius: 30px;

    background-image: linear-gradient(rgba(0, 0, 0, 0.3),rgba(0, 0, 0, 0.3)) , url("/src/assets/card-bg.jpeg");
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center center;
}

.subcard-text {
    font: 550 18px Avenir;
    text-align: start;
    color: #fff;
    padding: 30px;
}

.contact-me {
    font-size: 1.2rem;
    width: 50%;
    background-color: #fff;
    border-radius: 10px;
    padding: 20px;
    margin: 2rem 0;
}
</style>
