<template>
    <div class="contact">
        <section>
            <h2>Skontaktuj się z nami!</h2>
            <p><a href="mailto:info@example.com">fizjostacja.bochnia@gmail.com</a></p>
            <p><a href="tel:+48780605484">+48780605484</a></p>
            <p>Trudna 20/2, 32-700 Bochnia</p>
            <p>Godziny otwarcia: <br> Od poniedziałku do piątku, 6:00 - 23:00</p>
            <p>Istnieje możliwość umówienia wizyty w weekendy i święta po wcześniejszym kontakcie telefonicznym.</p>
        </section>
        <button @click="goTop">Wróć na górę</button>
    </div>
    <div class="maps">
        <h2>Odwiedź nas!</h2>
        <h3>Za budynkiem znajduję się bezpłatny parking dla pacjentów</h3>
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

    a {
        text-decoration: none;
        color: cornflowerblue;
        font-weight: bold;
    }
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
    width: 20vh;
}

button:hover {
    cursor: pointer;
}

</style>