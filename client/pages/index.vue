<template>
    <main>
        <section class="videotitle">
            <video src="http://localhost:1337/uploads/Galactic_Spiral_4_K_Motion_Background_Loop_c66bf3ed90.mp4" autoplay loop muted></video>
            <h1 class="title">Добро пожаловать в мир психологии и саморазвития!</h1>
        </section>
    </main>
</template>

<style scoped>
    .videotitle {
        width: 100%;
        height: 100vh;
        position: relative;
    }
    .videotitle video {
        width: 100%;
        height: 100%;
        position: absolute;
        top: 0;
        left: 0;
        object-fit: cover;
    }
    .title {
        width: 100%;
        height: 100%;
        background-color: black;
        font-family: Georgia, 'Times New Roman', Times, serif;
        font-size: 100px;
        color: white;
        mix-blend-mode: multiply;
    }
</style>
