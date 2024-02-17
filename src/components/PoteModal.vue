<template>
    <div class="modal-body" v-if="this.isOpen" @close="openModal = false">

        <div class="text-container">
            <p>
                write me a mail:
            </p>
            <a href="mailto:o.jpkmc@gmail.com?subject=Subject%20of%20the%20Email&body=Body%20of%20the%20Email">
                <p id="copy-cat">
                    o.jpkmc@gmail.com
                </p>
                <button @click="copyText">ctrl+c</button>
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
            document.execCommand("copy");
            document.body.removeChild(textarea);
        },


    }
};
</script>
  
<style lang="scss" scoped>
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
            animation: animate 15s ease-in-out infinite;
            font-weight: 1000;

            -webkit-text-stroke: 0.05rem greenyellow;

            @media only screen and (max-width: 600px) {
                font-size: 9vw;
                -webkit-text-stroke: 0.02rem greenyellow;

            }
        }


        a {
            text-decoration: none;
        }

        button {
            transform: rotate(.15rad);
            margin: 0 0 0 25vh;
            padding: 8px 8px 8px 8px;
            border-radius: 10px;
            font-size: 1.5vh;
            font-weight: 600;
            cursor: pointer;
        }

        @keyframes animate {

            0%,
            100% {
                background-position: left top;
            }

            25% {
                background-position: right bottom;
            }

            50% {
                background-position: left bottom;
            }

            75% {
                background-position: right top;
            }

        }
    }

}
</style>
