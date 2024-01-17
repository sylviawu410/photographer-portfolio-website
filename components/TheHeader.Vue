<template>
    <header class="header">
        <div class="nav-bar">
            <ul>
                <li>
                    <nuxt-link to="/">
                        <div class="logo"><img src="~assets/image/logo.png" /></div>
                    </nuxt-link>
                </li>
                <li>
                    <ul>
                        <li>
                            <nuxt-link to="/">Home</nuxt-link>
                        </li>
                        <li>
                            <nuxt-link to="/about-me">About Me</nuxt-link>
                        </li>
                        <li>
                            <nuxt-link to="/portfolio">Portfolio</nuxt-link>
                        </li>
                        <li>
                            <nuxt-link to="/services">Services</nuxt-link>
                        </li>
                    </ul>
                </li>
                <li>
                    <nuxt-link to="contact-page">
                        <div class="contact-btn">Contact Me</div>
                    </nuxt-link>
                </li>

            </ul>
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
        padding: 0px 125px;
        flex-direction: column;
        align-items: flex-start;
        gap: 10px;
        border-bottom: 1px solid var(--Dark-12, #1C1C21);

    }

    .header .nav-bar {
        /* width: 86.97%; */
        width: 91.38%;
        display: flex;
        padding: 30px 40px;
        /* justify-content: space-between;
        align-items: center;
        align-self: stretch; */
        border-right: 1px solid var(--Dark-12, #1C1C21);
        border-left: 1px solid var(--Dark-12, #1C1C21);
    }

    .header .logo img {
        width: 134.1px;
        height: 27px;
        margin: 0 352.9px 0 0;

    }

    .header a {
        text-decoration: none;
        color: white;
        cursor: pointer;
    }

    .header ul {
        list-style: none;
        display: flex;
    }

    .header .contact-btn {
        margin-right: 18px;
        display: flex;
        padding: 16px 24px;
        align-items: center;
        gap: 10px;
        border-radius: 10px;
        border: 1px solid #2F2F37;
        background: var(--Dark-12, #1C1C21);
    }
}

@media screen and (min-width:1440px) {
    .header .nav-bar {
        width: 86.97%;
    }

    
}
</style>