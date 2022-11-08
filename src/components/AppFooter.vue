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

    <div class="footer-bg-down">
        <div class="footer-down">

            <div class="btn-footer">
                <div class="btn">SIGN-UP NOW</div>
            </div>

            <div class="social-footer">
                FOLLOW US
                <img src="../assets/img/footer-facebook.png" alt="">
                <img src="../assets/img/footer-twitter.png" alt="">
                <img src="../assets/img/footer-facebook.png" alt="">
                <img src="../assets/img/footer-youtube.png" alt="">
                <img src="../assets/img/footer-pinterest.png" alt="">
                <img src="../assets/img/footer-periscope.png" alt="">
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

.footer-bg-down {
    background-color: #303030;
}


.footer-down {
    width: 90%;
    margin: auto;
    max-width: 1200px;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    padding: 2rem;
    align-items: center;
    background-color: #303030;

    .btn {
        border: 3px solid #0082f9;
        padding: .8rem;
        color: white;
        cursor: pointer;
    }
}

.social-footer {
    color: #0082f9;
    display: flex;
    align-items: center;
    gap: .5rem;
}
</style>