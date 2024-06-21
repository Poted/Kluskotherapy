<template>
    <div class="contact">
        <section>
            <h2>Kontakt</h2>
            <div class="hyperlynx"><p><a href="mailto:info@example.com">fizjostacja.bochnia@gmail.com</a></p></div>
            <div class="hyperlynx"><p><a href="tel:+48780605484">+48780605484</a></p></div>
            <div class="hyperlynx"><p><a href="https://maps.google.com/maps?ll=49.971895,20.432447&z=17&t=m&hl=pl-PL&gl=US&mapclient=embed&cid=4526446267161382639">Trudna 20/2, 32-700 Bochnia</a></p></div>
            <br>
            <p><strong>Godziny otwarcia: <br> Od poniedziałku do piątku,<br>6:00 - 23:00</strong></p>
            <p>Istnieje możliwość umówienia wizyty w weekendy i święta po wcześniejszym kontakcie telefonicznym.</p>
        </section>
        <button @click="goTop">↑ Wróć na górę ↑</button>
    </div>
    <div class="maps">
        <h2>Odwiedź nas!</h2>
        <h3>Za budynkiem znajduje się bezpłatne miejsce parkingowe dla pacjentów</h3>
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

<style scoped lang="scss">

.contact {
    margin-top: 10px;
    font-size: 18px;
    
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    
    .hyperlynx {

        width: 80%;
        margin: 0px 10%;
        

        p {
            
            border: 1px solid black;
            border-radius: 10px;
            box-shadow: 0px 0px 5px 1px #b1b1b1b2;
            background-color: #f1f1f1;
            padding: 20px;
            
            a {
                text-decoration: none;
                color: cornflowerblue;
                font-weight: bold;
            }
            
        }
        
        @media only screen and (min-width: 1024px) {
            font-size: 22px;
            width: 50%;
            margin-left: 25%;
        }
    }


}

.maps {
    margin-top: 60px;
    text-align: center;
}

button {

    font-family: "M PLUS Rounded 1c", sans-serif;
    font-weight: 900;
    font-style: normal;
  

    border: none;
    outline: none;
    padding: 10px 25px;
    border-radius: 15px;
    color: #333;
    background: #fff;
    box-shadow: 0 3px 20px 0 #0000003b;
    margin-top: 40px;
}

button:hover {
    cursor: pointer;
}

</style>