<template>
    <div class="about-me-page">
        <div class="section1">
            <div class="background">
                <img class="background-pic" src="~assets/image/about-me-page.png">
                <div class="overlay">
                    <div class="section1-left">
                        <div class="section1-text">About</div>
                        <h1 class="section1-heading">Damien Braun</h1>
                    </div>
                    <div class="section-middle">
                        <div class="items">
                            <div class="title">15+</div>
                            <div class="text">Years in Business</div>
                        </div>
                        <div class="items">
                            <div class="title">500+</div>
                            <div class="text">Happy Clients</div>
                        </div>
                        <div class="items">
                            <div class="title">10+</div>
                            <div class="text">Photography Awards</div>
                        </div>
                        <div class="items">
                            <div class="title">05+</div>
                            <div class="text">International Shoots</div>
                        </div>
                        <div class="items">
                            <div class="title">10,000+</div>
                            <div class="text">Social Media Followers</div>
                        </div>
                        <div class="items">
                            <div class="title">90%</div>
                            <div class="text">Client Retention Rate</div>
                        </div>
                    </div>
                    <div class="bottom-pic">
                        <img class="star" src="~assets/image/star-with-circle.svg">
                        <div class="text">Scroll Down To See My Journey</div>
                    </div>
                    <div class="bottom">
                        <div class="title">My Biography</div>
                        <div class="text">Damien Braun's love affair with photography began at a young age, nurtured by the captivating landscapes and vibrant cultures surrounding her in the heart of the USA. Her passion for storytelling through imagery led her to embark on a photography journey that has spanned over 15 years.
Driven by an insatiable curiosity to explore the beauty in everyday moments, Damien has honed her craft meticulously. Her background in digital media provided her with a solid foundation, but it's her keen eye for detail and an innate ability to capture raw emotions that truly set her apart.
Damien's journey is more than just taking pictures; it's about capturing the essence of the human spirit, the fleeting magic of nature, and the emotions that define our lives. With each click of her camera, she weaves stories that transcend time and space.</div>
                    </div>
                </div>
            </div>
        </div>
        <div class="section2">
            
        </div>
    </div>
</template>

<style>
.about-me-page {
    width: 100%;
    padding-bottom: 562px;
}

.about-me-page .section1 {
    display: flex;
    padding: 0 80px;
    align-items: center;
    height: 100%;
    position: relative;
    margin-top: 80px;

}

.about-me-page .section1-left {
    margin-bottom: 24px;
}

.about-me-page .section1-text {
    color: var(--Grey-40, #62646C);
    font-size: 18px;
    font-weight: 600;
    line-height: normal;
    font-style: normal;
    text-transform: uppercase;
}

.about-me-page .section1-heading {
    font-size: 48px;
}

.about-me-page .section1 .background {
    position: relative;
    z-index: 1;
}

.about-me-page .section1 .background-pic {
    height: 100%;
    width: 100%;
}

.about-me-page .section1 .overlay {
    position: absolute;
    top: 0;
    left: 0;
    display: flex;
    justify-content: center;
    align-items: start;
    flex-direction: column;
    z-index: 2;
    width: 100%
}

.about-me-page .section1 .section-middle {
    display: flex;
    align-items: flex-start;
    gap: 10px;
    align-self: stretch;
    justify-content: space-around;
}

.about-me-page .section1 .section-middle .items {
    display: flex;
    padding: 20px 24px;
    flex-direction: column;
    align-items: flex-start;
    flex: 1 0 0;
    border-radius: 12px;
    border: 1px solid var(--Dark-12, #1C1C21);
    background: var(--Dark-06, #0E0E10);
}

.about-me-page .section1 .section-middle .title {
    color: var(--Absolute-White, #FFF);
    font-family: Manrope;
    font-size: 34px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
    text-transform: uppercase;
}

.about-me-page .section1 .section-middle .text {
    color: var(--Grey-50, #797C86);
    font-family: Manrope;
    font-size: 14px;
    font-style: normal;
    font-weight: 400;
    line-height: 150%;
    /* 21px */
}

.about-me-page .section1 .bottom-pic {
    display: flex;
    padding: 18px 20px;
    justify-content: space-between;
    align-items: center;
    align-self: stretch;
    margin-top: 271px;
}

.about-me-page .section1 .bottom-pic .text {
    width: 164px;
    color: var(--Grey-50, #797C86);
    font-size: 14px;
    text-transform: uppercase;
}

.about-me-page .section1 .bottom{
    margin-top: 80px;
    display: flex;
padding: 60px 0px;
flex-direction: column;
align-items: flex-start;
gap: 30px;
align-self: stretch;
border-top: 1px solid var(--Dark-12, #1C1C21);
border-bottom: 1px solid var(--Dark-12, #1C1C21);
}

.about-me-page .section1 .bottom .title{
    color: var(--Grey-50, #797C86);
font-size: 34px;
font-weight: 600;
text-transform: uppercase;
}

.about-me-page .section1 .bottom .text {

}
</style>