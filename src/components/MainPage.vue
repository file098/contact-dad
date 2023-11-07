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
    </div>
    <div class="description">
        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Nam
        praesentium tenetur et pariatur. Ipsum voluptatum quisquam labore ipsam
        sunt vel sed illo dolor optio ratione officiis voluptas mollitia, dolore
        eos.
    </div>
    <button class="contact-me">Contattami</button>
    <!-- <iframe class="komoot-iframe" src="https://www.komoot.com/user/3227558101012/embed?stats=1" width="640" height="580" frameborder="0" scrolling="no"></iframe> -->
</template>
<script>
export default {
    name: "MainPage",
};
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700&display=swap');

body {
    font-family: 'Poppins', sans-serif;
}

.card {
    position: relative;
    height: 60vh;
    display: flex;
    flex-direction: column;
    justify-content: end;

    color: #fff;
    background-image: linear-gradient(rgba(0, 0, 0, 0.3), rgba(0, 0, 0, 0.3)), url("/src/assets/card-bg.jpeg");
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center center;

    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.50);
    border-radius: 50px;

    .header {
        margin-top: 2rem;
        display: flex;
        flex-flow: column;
        text-align: start;
        margin: 2rem;

        .card-title {
            font: 550 48px Poppins;
            text-transform: uppercase;
        }

        .card-subtitle {
            font: 400 16px Poppins;
        }
    }
}

.description {
    font: 1.2rem Poppins;
    background-color: #fff;
    padding: 20px;
    text-align: start;
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
    background: linear-gradient(180deg, rgba(142,205,60,1) 0%, rgba(108,171,39,1) 100%);
    color: white;
    border: none;
    cursor: pointer;
}
</style>
