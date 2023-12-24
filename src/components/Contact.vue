<template>
    <div class="contact">
        <section>
            <h2>Skontaktuj się z nami!</h2>
            <p>Email: <a href="mailto:info@example.com">julka@jestsuperfizjo.com</a></p>
            <p>Telefon: <a href="tel:+48606761989">+48 606 761 989</a></p>
            <p>Adres: Trudna 22, 32-700 Bochnia</p>
            <p>Godziny otwarcia: Od poniedziałku do piątku, 9:00 - 18:00</p>
        </section>
    </div>
    <div class="maps">
        <h2>Odwiedź nas!</h2>

        <Maps />
    </div>
</template>

<script setup>
import Maps from './Maps.vue'
</script>

<style scoped lang="scss">

    .contact {

        section {

            
            display: flex;
            flex-direction: column;
            align-content: center;
        }
    }


</style>