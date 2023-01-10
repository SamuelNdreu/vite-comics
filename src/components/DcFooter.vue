<script>
export default {

    data() {
        return {
            dcComics: [
                {
                    text: 'Characters'
                },
                {
                    text: 'Comics'
                },
                {
                    text: 'Movies'
                },
                {
                    text: 'Tv'
                },
                {
                    text: 'Games'
                },
                {
                    text: 'Videos'
                },
                {
                    text: 'News'
                },
            ],
            dc: [
                {
                    text: 'Terms Of Use'
                },
                {
                    text: 'Privacy policy (News)'
                },
                {
                    text: 'Ad Chpoces'
                },
                {
                    text: 'Advertising'
                },
                {
                    text: 'Jobs'
                },
                {
                    text: 'Subscriptions'
                },
                {
                    text: 'Talent Workshops'
                },
                {
                    text: 'CPSC Certificates'
                },
                {
                    text: 'Ratings'
                },
                {
                    text: 'Shop Help'
                },
                {
                    text: 'Contact Us'
                },
            ],
            sites: [
                {
                    text: 'DC'
                },
                {
                    text: 'MAD Magazine'
                },
                {
                    text: 'DC Kids'
                },
                {
                    text: 'DC Universe'
                },
                {
                    text: 'DC Power Visa'
                },
            ],
            shop: [
                {
                    text: 'Shop DC'
                },
                {
                    text: 'Shop DC Collectibles'
                },
            ],
        }
    },
}
</script>

<template>
    <section class="top-footer">
        <div class="container">
            <div class="footer-links ">
                <ul>
                    <li>
                        <h2>DC comics</h2>
                    </li>
                    <li v-for="items in dcComics">{{ items.text }}</li>
                    <li>
                        <h2>Shop</h2>
                    </li>
                    <li v-for="items in shop">{{ items.text }}</li>
                </ul>
                <ul>
                    <li>
                        <h2>DC</h2>
                    </li>
                    <li v-for="items in dc">{{ items.text }}</li>
                </ul>
                <ul>
                    <li>
                        <h2>Sites</h2>
                    </li>
                    <li v-for="items in sites">{{ items.text }}</li>
                </ul>
                <ul>

                </ul>
            </div>
        </div>
    </section>
    <section class="bottom-footer">
        <div class="footer-wrapper">
            <div class="container footer-flex">
                <button>sign-up now!</button>
                <div class="social">
                    <span>Follow Us</span>
                    <img src="../assets/img/footer-facebook.png" alt="facebook">
                    <img src="../assets/img/footer-twitter.png" alt="twitter">
                    <img src="../assets/img/footer-youtube.png" alt="youtube">
                    <img src="../assets/img/footer-pinterest.png" alt="pinterest">
                    <img src="../assets/img/footer-periscope.png" alt="periscope">
                </div>
            </div>

        </div>

    </section>

</template>

<style>
.top-footer {
    background-image: url('../assets/img/footer-bg.jpg');
    background-size: cover;
}

.footer-links {
    display: flex;
    width: 60%;
    padding: 3rem;
}

ul {
    list-style-type: none;
    margin-right: 1.5rem;
}

ul li {
    line-height: 1.6;
    font-size: .9rem;
    color: #848484;
    font-weight: 700;
}

li h2 {
    color: white;
    text-transform: uppercase;
    font-size: 1.2rem;
    margin: 1rem 0;
}

.footer-wrapper {
    height: 8rem;
    background-color: #303030;
    color: white;
    z-index: 2;
}

.footer-flex {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.social {
    margin-top: 2rem;
}

    span {
        text-transform: uppercase;
        font-size: 1.5rem;
        font-weight: bolder;
        color: #0282f9;
        vertical-align: baseline;
    }

    img {
        padding-left: 1rem;
    }

button {
    margin-top: 2rem;
    padding: 1rem;
    text-transform: uppercase;
    background-color: transparent;
    color: white;
    font-size: large;
    border: 3px solid #0282f9;
}
</style>