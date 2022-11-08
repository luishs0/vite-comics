<script>
export default {
    name: "AppFooter",
    data() {
        return {

        }
    }
}
</script>


<template>
    <div class="container-bg-footer">
        <div class="container-footer">
            <div class="footer-text">
                <div class="col-1">
                    <h3>DC COMICS</h3>
                    <ul>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>TV</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                    </ul>
                    <h3>SHOP</h3>
                    <ul>
                        <li>Shop DC</li>
                        <li>Shop DC Collectibles</li>
                    </ul>
                </div>
                <div class="col-2">
                    <h3>DC</h3>
                    <ul>
                        <li>Lorem</li>
                        <li>Ipsum</li>
                        <li>Dolor</li>
                        <li>lorem</li>
                        <li>Lorem</li>
                        <li>Lorem</li>
                        <li>Lorem</li>
                        <li>Lorem</li>
                        <li>Lorem</li>
                        <li>Lorem</li>
                        <li>Lorem</li>
                    </ul>
                </div>
                <div class="col-3">
                    <h3>SITES</h3>
                    <ul>
                        <li>DC</li>
                        <li>MAD Magazine</li>
                        <li>DC Kids</li>
                        <li>DC Universe</li>
                        <li>DC Power Visa</li>
                    </ul>
                </div>
            </div>

            <div class="footer-img">
                <img src="../assets/img/dc-logo-bg.png" alt="">
            </div>
        </div>
    </div>
</template>


<style lang="scss" scoped>
.container-footer,
.footer-text {
    display: flex;
    flex-wrap: wrap;
}

.container-bg-footer {
    background-image: url(../assets/img/footer-bg.jpg);
    background-size: cover;
}

.container-footer {
    width: 90%;
    margin: auto;
    justify-content: space-between;
    align-items: center;
    max-width: 1200px;
}

.footer-text {
    color: white;
    justify-content: flex-start;
    gap: 1.5rem;
    width: 50%;

    ul,
    h3 {
        margin-bottom: 1rem;
    }


}

.footer-img {
    width: 50%;

    img {
        object-fit: cover;
    }
}

ul {
    list-style-type: none;
}
</style>