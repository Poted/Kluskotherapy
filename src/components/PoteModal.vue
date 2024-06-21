<template>
    <div class="modal-body" v-if="this.isOpen" @close="openModal = false">

        <div class="text-container">
            <p>
                napisz do nas:
            </p>
            <div class="mail">
                <p>
                    <a href="mailto:o.jpkmc@gmail.com?subject=Subject%20of%20the%20Email&body=Body%20of%20the%20Email">
                        o.jpkmc@gmail.com
                    </a>
                </p>
            </div>
            <p>
                lub zadzwoń:
            </p>
            <a href="tel:+48788455086">
                    <p>
                    +48788455086
                </p>
                </a>
        </div>

    </div>
</template>
  
<script>
export default {
    data() {
        return {
            isOpen: false
        };
    },
    methods: {
        openModal() {
            this.isOpen = !this.isOpen;
        },
        copyText() {
            const textToCopy = "o.jpkmc@gmail.com";
            const textarea = document.createElement("textarea");
            textarea.value = textToCopy;
            document.body.appendChild(textarea);
            textarea.select();
            // document.execCommand("copy");
            document.body.removeChild(textarea);
        },


    }
};
</script>
  
<style lang="scss" scoped>

@keyframes text-background {

0% {
// 100% {
    background-position: left top;
}

// 25% {
//     background-position: left bottom;
// }

// 50% {
//     background-position: left top;
// }

100% {
// 75% {
    background-position: left bottom;
}

}



.modal-body {
    margin: 0;
    padding: 0;
    font-family: 'Raleway', sans-serif;

    .text-container {
        width: 90vw;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;

        p {
            margin: 0;
            font-size: 4vw;
            color: rgba(0, 0, 0, .0);
            background-image: url("https://png.pngtree.com/background/20230612/original/pngtree-dark-fractal-wallpaper-by-kristine-schiltz-picture-image_3173399.jpg");
            background-repeat: repeat;
            -webkit-background-clip: text;
            background-clip: text;
            animation: text-background 3s linear infinite;
            font-weight: 1000;

            -webkit-text-stroke: 0.05rem greenyellow;

            @media only screen and (max-width: 600px) {
                font-size: 9vw;
                -webkit-text-stroke: 0.02rem greenyellow;
            }

        }


        a {
            text-decoration: none;
            color: blue;
            font-weight: 700;

        }



    }

}
</style>
