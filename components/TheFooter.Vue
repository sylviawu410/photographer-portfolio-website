<template>
    <footer class="footer">
        <div class="logo-container">
            <img src="~assets/image/Damien.svg">
        </div>
        <div class="scroll-container">
            <div class="scroll-text">
                <div class="scroll-item">
                    <img src="~assets/image/star.svg">
                    <span>Comercial Photography</span>
                </div>
                <div class="scroll-item">
                    <img src="~assets/image/star.svg">
                    <span>Product Photography</span>
                </div>
                <div class="scroll-item">
                    <img src="~assets/image/star.svg">
                    <span>Wedding Photography</span>
                </div>
                <div class="scroll-item">
                    <img src="~assets/image/star.svg">
                    <span>Landscape Photography</span>
                </div>
                <div class="scroll-item">
                    <img src="~assets/image/star.svg">
                    <span>Branding Photography</span>
                </div>
                <div class="scroll-item">
                    <img src="~assets/image/star.svg">
                    <span>Portrait Photography</span>
                </div>
            </div>
        </div>
        <div class="upper-section">
            <div class="background-left"><img src="~assets/image/background.png" /></div>
            <div class="container-left">
                <div class="container-left-text">A MORE MEANINGFUL HOME FOR PHOTOGRAPHY</div>
                <div class="container-left-wrapper">
                    <h1>Let’s</h1>
                    <div class="purple-btn">
                        <div class="purple-btn-background"></div>
                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
                            <path fill-rule="evenodd" clip-rule="evenodd"
                                d="M8.25 3.75L19.5 3.75C19.6989 3.75 19.8897 3.82902 20.0303 3.96967C20.171 4.11032 20.25 4.30109 20.25 4.5V15.75C20.25 16.1642 19.9142 16.5 19.5 16.5C19.0858 16.5 18.75 16.1642 18.75 15.75V6.31066L5.03033 20.0303C4.73744 20.3232 4.26256 20.3232 3.96967 20.0303C3.67678 19.7374 3.67678 19.2626 3.96967 18.9697L17.6893 5.25L8.25 5.25C7.83579 5.25 7.5 4.91421 7.5 4.5C7.5 4.08579 7.83579 3.75 8.25 3.75Z"
                                fill="white" />
                        </svg>
                    </div>
                </div>
                <h1>Work Together</h1>
            </div>
            <div class="container-right">
                <div class="container-right-box">
                    <div class="container-right-heading">Home</div>
                    <nuxt-link to="/about-me-page">
                        <div class="container-right-text">About Me</div>
                    </nuxt-link>
                    <nuxt-link to="/portfolio-page">
                        <div class="container-right-text">My Works</div>
                    </nuxt-link>
                    <nuxt-link to="/services-page">
                        <div class="container-right-text">Testimonials</div>
                    </nuxt-link>
                </div>

                <div class="container-right-box">
                    <div class="container-right-heading">Clients</div>
                    <div class="container-right-text">Klovesto</div>
                    <div class="container-right-text">Nukeway</div>
                    <div class="container-right-text">Cloven’s</div>
                    <div class="container-right-text">MenVol</div>
                </div>

                <div class="container-right-box">
                    <div class="container-right-heading">Portfolio</div>
                    <nuxt-link to="/portfolio-page#Events"><div class="container-right-text">Events</div></nuxt-link>
                    <nuxt-link to="/portfolio-page#Portrait"><div class="container-right-text">Portrait</div></nuxt-link>
                    <nuxt-link to="/portfolio-page#Commerciale"><div class="container-right-text">Commerciale</div></nuxt-link>
                </div>
                <div class="container-right-box">
                    <div class="container-right-heading">Services</div>
                    <nuxt-link to="/services-page#Portraits"><div class="container-right-text">Portraits</div></nuxt-link>
                    <nuxt-link to="/services-page#Events"><div class="container-right-text">Events</div></nuxt-link>
                    <nuxt-link to="/services-page#Commercial"><div class="container-right-text">Commercial</div></nuxt-link>
                </div>
            </div>
            <div class="background-right"><img src="~assets/image/background.png" /></div>
        </div>
        <div class="lower-section">
            <div class="lower-section-text-wrapper">
                <div class="lower-section-text-terms">Terms & Conditions</div>
                <div class="lower-section-text-privacy">Privacy Policy</div>
            </div>
            <div class="lower-scetion-wrapper">
                <img class="lower-section-logo" src="~assets/image/facebook.png" />
                <img class="lower-section-logo" src="~assets/image/twitter.png" />
                <img class="lower-section-logo" src="~assets/image/linkedin.png" />
            </div>
            <div class="lower-section-text-rights">© 2024 Damien Braun Photography. All rights reserved.</div>
        </div>
    </footer>
</template>

<style>
@media screen and (max-width: 992px) {
    .footer {
        display: none;
    }
}

@media screen and (min-width: 992px) {
    .footer {
        width: 100%;
        bottom: 0;
        position: relative;
        z-index: 1;
        overflow: hidden;
    }

    .footer .logo-container {
        display: flex;
        margin-right: 80px;
        flex-direction: column;
        align-items: flex-end;
        margin-bottom: 60px;
    }

    .footer .scroll-container {
        overflow: hidden;
        padding: 16px;
        border-top: 1px solid var(--Dark-12, #1C1C21);
        border-bottom: 1px solid var(--Dark-12, #1C1C21);
        background: var(--Dark-06, #0E0E10);

    }

    .footer .scroll-text {
        font-size: 14px;
        display: flex;
        gap: 16px;

        -moz-transform: translateX(100%);
        -webkit-transform: translateX(100%);
        transform: translateX(100%);

        -moz-animation: my-animation 15s linear infinite;
        -webkit-animation: my-animation 15s linear infinite;
        animation: my-animation 15s linear infinite;
    }

    .footer .scroll-item {
        display: flex;
        align-items: center;
        gap: 6px;
    }

    .footer .scroll-item img {
        width: 30px;
        height: 30px;
    }

    .footer .scroll-item span {
        text-align: center;
    }

    @keyframes my-animation {
        from {
            -moz-transform: translateX(-100%);
            -webkit-transform: translateX(-100%);
            transform: translateX(100%);
        }

        to {
            -moz-transform: translateX(100%);
            -webkit-transform: translateX(100%);
            transform: translateX(-100%);
        }

    }

    .footer .upper-section {
        min-height: 368px;
        display: flex;
        justify-content: space-between;
        align-items: center;
        position: relative;
    }

    .footer .background-left img {
        max-width: 100%;
        max-height: 100%;
    }

    .footer .background-left {
        width: 187px;
        height: 187px;
        position: absolute;
        left: -107px;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .footer .container-left {
        flex: 1;
        display: flex;
        justify-content: center;
        flex-direction: column;
        align-items: flex-start;
        padding: 80px 60px 80px 140px;
        /* align-self: stretch; */
    }

    .footer .container-left-text {
        color: var(--Grey-50, #797C86);
        font-size: 16px;
        font-weight: 600;
        line-height: normal;
        padding-bottom: 50px;
        font-style: normal;
    }

    .footer .container-left-wrapper {
        width: 100%;
    }

    .footer h1 {
        float: left;
        clear: none;
    }

    .footer a {
        text-decoration: none;
        color: white;
        cursor: pointer;
    }

    .footer .purple-btn {
        float: inline-start;
        clear: none;
        margin-left: 12px;
        margin-top: 5px;
        position: relative;
        width: 104px;
        height: 56px;
        top: 0;
        left: 0;
    }

    .footer .purple-btn-background {
        display: flex;
        padding: 28px 50px;
        align-items: center;
        gap: 10px;
        border-radius: 100px;
        background: var(--Purple-55, #4A2CED);
        box-shadow: 4px 4px 17.4px 0px rgba(255, 255, 255, 0.28) inset;
        position: relative;
        top: 0;
        left: 0;
    }

    .footer svg {
        position: absolute;
        top: 16px;
        left: 40px;
    }

    .footer .container-right {
        display: flex;
        flex-wrap: wrap;
        padding: 80px 130px 80px 50px;
        justify-content: space-between;
        align-items: flex-start;
        flex: 1 0 0;
    }

    .footer .container-right-box {
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        padding: 6px 0px;
        gap: 10px;
    }

    .footer .container-right-heading {
        color: var(--Grey-50, #797C86);
        font-size: 14px;
        font-weight: 600;
        line-height: normal;
        text-transform: uppercase;
        padding-bottom: 12px;
    }

    .footer .container-right-text {
        color: var(--Grey-95, #F2F2F3);
        font-size: 14px;
        font-style: normal;
        font-weight: 500;
        line-height: normal;
        text-transform: uppercase;
    }


    .footer .background-right {
        width: 187px;
        height: 187px;
        transform: rotate(180deg);
        position: absolute;
        right: -107px;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .footer .background-right img {
        max-width: 100%;
        max-height: 100%;
    }

    .footer .lower-section {
        display: flex;
        padding: 34px 80px;
        justify-content: space-between;
        align-items: center;
    }

    .footer .lower-section-text-wrapper {
        display: flex;
        align-items: center;
        gap: 8px;
    }

    .footer .lower-section-text-terms,
    .lower-section-text-privacy {
        float: left;
        clear: none;
        color: var(--Grey-50, #797C86);
        font-size: 14px;
        font-style: normal;
        font-weight: 400;
        line-height: 150%;

    }

    .footer .lower-section-text-rights {
        color: var(--Grey-50, #797C86);
        font-size: 14px;
        font-style: normal;
        font-weight: 400;
        line-height: 150%;

    }

    .footer .lower-scetion-wrapper {
        display: flex;
        padding: 8px;
        justify-content: flex-end;
        gap: 8px;
        border-radius: 100px;
        border: 1px solid var(--Dark-12, #1C1C21);
        background: var(--Dark-03, #070708);
    }

    .footer .lower-section-logo {
        width: 18px;
        height: 18px;
        padding: 10px;
        border-radius: 100px;
        border: 1px solid #2F2F37;
        background: var(--Dark-12, #1C1C21);
    }


}
</style>