<template>
    <header class="header">
        <div class="nav-bar">
            <li>
                <nuxt-link to="/">
                    <div class="logo"><img src="~assets/image/logo.png" /></div>
                </nuxt-link>
            </li>
            <li>
                <ul class="page-btn-container">
                    <li>
                        <nuxt-link to="/">
                            <div class="page-btn">Home</div>
                        </nuxt-link>
                    </li>
                    <li>
                        <nuxt-link to="/about-me-page">
                            <div class="page-btn">About Me</div>
                        </nuxt-link>
                    </li>
                    <li>
                        <nuxt-link to="/portfolio-page">
                            <div class="page-btn">Portfolio</div>
                        </nuxt-link>
                    </li>
                    <li>
                        <nuxt-link to="/services-page">
                            <div class="page-btn">Services</div>
                        </nuxt-link>
                    </li>
                </ul>
            </li>
            <li>
                <nuxt-link to="contact-page">
                    <div class="contact-btn">Contact Me</div>
                </nuxt-link>
            </li>

        </div>
    </header>
</template>

<script></script>

<style>
@media screen and (max-width:992px) {
    .header {
        display: none;
    }
}

@media screen and (min-width:992px) {
    .header {
        display: flex;
        width: 100%;
        max-height: 89px;
        position: relative;
        justify-content: center;
        border-bottom: 1px solid var(--Dark-12, #1C1C21);
        z-index: 1;
        top: 0
    }

    .header .nav-bar {
        min-width: 1280px;
        max-height: 89px;
        display: flex;
        border-right: 1px solid var(--Dark-12, #1C1C21);
        border-left: 1px solid var(--Dark-12, #1C1C21);
        justify-content: space-between;
        align-self: stretch;
        color: var(--Grey-70, #AFB0B6);
        font-size: 14px;
        font-style: normal;
        font-weight: 500;
        line-height: 150%;
    }

    .header .logo img {
        width: 109.267px;
        height: 22px;
        margin: 0 352.9px 0 0;
        padding: 33.5px 18px;

    }

    .header a {
        text-decoration: none;
        color: white;
        cursor: pointer;
    }

    .header li {
        list-style: none;
        display: flex;
        align-items: center;
        margin: 0;
        padding: 0;

    }

    .header ul {
        list-style: none;
        display: flex;
        /* align-items: center; */
        margin: 0;
        padding: 0;

    }

    .header .page-btn-container {
        display: flex;
        align-items: center;
        position: absolute;
        right: 419.5px;
        bottom: 0px;
        border-radius: 10px 10px 0px 0px;
        border-top: 1px solid var(--Dark-12, #1C1C21);
        border-right: 1px solid var(--Dark-12, #1C1C21);
        border-left: 1px solid var(--Dark-12, #1C1C21);
    }

    .header .page-btn {
        display: flex;
        padding: 24px 40px;
        align-items: center;
        gap: 10px;
        border-right: 1px solid var(--Dark-12, #1C1C21);
        border-left: 1px solid var(--Dark-12, #1C1C21);
        /* background: var(--Dark-08, #131316); */
    }

    .header .contact-btn {
        display: flex;
        padding: 14px 20px;
        align-items: center;
        gap: 10px;
        border-radius: 8px;
        border: 1px solid #2F2F37;
        background: var(--Dark-12, #1C1C21);
    }
}

/* @media screen and (min-width:1440px) {
    .header .nav-bar {
        width: 86.97%;
    }


} */
</style>