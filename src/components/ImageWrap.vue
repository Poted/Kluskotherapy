<template>
    <div class="img-wrap">
        <div class="white-border">
            <!-- <img src="https://scontent-waw1-1.xx.fbcdn.net/v/t1.15752-9/403394328_890183829072000_4380863316342879423_n.jpg?_nc_cat=104&ccb=1-7&_nc_sid=8cd0a2&_nc_ohc=HifIKnoIv30AX97I3aX&_nc_ht=scontent-waw1-1.xx&oh=03_AdRW8nM_e2UYA77Fhn9tqNK21-SLTmw_UnZgmaAn8xTqJg&oe=65B0DB88" -->
            <img src="../../public/salon.jpg"
                alt="salon" />
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            distance: 46,
            thickness: 3,
        };
    },
    methods: {
        updateDistance() {
            this.$refs.wrap.style.setProperty(
                '--distance',
                `${this.distance}%`
            );
        },
        updateThickness() {
            this.$refs.wrap.style.setProperty(
                '--border',
                `${this.thickness}px`
            );
        },
    },
};
</script>


<style scoped>
.img-wrap {
    border-radius: 999px;
    background-color: #333;
    background-image: linear-gradient(80deg, #52e3593f 10%, #38456757 100%);
    width: 400px;
    height: 400px;
    display: flex;
    flex-direction: column;
    align-items: center;
}

.white-border {
    border-radius: 999px;
    background-color: #f1f1f1;
    width: 380px;
    height: 380px;


    display: flex;
    flex-direction: column;
    align-items: center;
    margin-top: 10px;

}

img {
    border-radius: 999px;
    margin-top: 10px;
    width: 360px;
    height: 360px;

}

@media only screen and (max-width: 600px) {

    .img-wrap {
        width: 300px;
        height: 300px;
    }

    .white-border {
        width: 280px;
        height: 280px;
    }

    img {
        width: 260px;
        height: 260px;
    }

}
</style>