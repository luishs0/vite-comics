<script>
export default {
    name: "AppBlueBar",
    data() {
        return {
            blueLinks: [
                {
                    name: "DIGITAL COMICS",
                    img: "buy-comics-digital-comics.png"
                },
                {
                    name: "DC MERCHANDISE",
                    img: "buy-comics-merchandise.png"
                },
                {
                    name: "SUBSCRIPTION",
                    img: "buy-comics-subscriptions.png"
                },
                {
                    name: "COMIC SHOP LOCATOR",
                    img: "buy-comics-shop-locator.png"
                },
                {
                    name: "DC POWER VISA",
                    img: "buy-dc-power-visa.svg"
                }
            ]
        }
    },
    methods: {
        getImagePath: function (imgPath) {
            return new URL(imgPath, import.meta.url).href;
        }
    }
}
</script>


<template>
    <div class="blue-bar">
        <div class="blue-bar-container">
            <ul>
                <li v-for="(blueLink, index) in blueLinks" :key="index">
                    <div class="li-img"> <img :src="getImagePath(`../assets/img/${blueLink.img}`)" alt="">
                    </div>
                    <div class="li-text"> {{ blueLink.name }} </div>
                </li>
            </ul>
        </div>
    </div>
</template>


<style lang="scss" scoped>
.blue-bar {
    background-color: #0082f9;
}

.blue-bar-container {
    width: 90%;
    margin: auto;
    max-width: 1200px;
}

ul {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;

    li {
        width: calc(100% / 5);
        list-style-type: none;
        color: white;
        padding: 2rem 0;
        display: flex;
        align-items: center;
        font-size: .8rem;

        .li-img {
            width: 30%;

            img {
                height: 40px;
                padding-right: .2rem;
            }
        }

        .li-text {
            width: 70%;
        }
    }
}
</style>