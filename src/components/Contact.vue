<template>
    <div class="contact">
        <section>
            <h2>Skontaktuj się z nami!</h2>
            <p><a href="mailto:info@example.com">julka@jestsuperfizjo.com</a></p>
            <p><a href="tel:+48666761989">+48 666 761 989</a></p>
            <p>Trudna 22, 32-700 Bochnia</p>
            <p>Godziny otwarcia: <br> Od poniedziałku do piątku, 9:00 - 18:00</p>
        </section>
        <button @click="goTop">Wróć na górę</button>
    </div>
    <div class="maps">
        <h2>Odwiedź nas!</h2>
        <Maps />
    </div>
</template>



<script setup>
import Maps from './Maps.vue'

const goTop = () => {
    window.scrollTo({
        top: 0,
        behavior: 'smooth',
    });
};

</script>

<style lang="scss">
// <style scoped lang="scss">

.contact {
    margin-top: 40px;
    text-align: center;
}

.maps {
    margin-top: 60px;
    text-align: center;
}

button {
    border: none;
    outline: none;
    padding: 10px 20px;
    border-radius: 50px;
    color: #333;
    background: #fff;
    box-shadow: 0 3px 20px 0 #0000003b;
    margin-top: 20px;
}

button:hover {
    cursor: pointer;
}

</style>