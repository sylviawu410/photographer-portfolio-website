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
                        <div class="text">Damien Braun's love affair with photography began at a young age, nurtured by
                            the captivating landscapes and vibrant cultures surrounding her in the heart of the USA. Her
                            passion for storytelling through imagery led her to embark on a photography journey that has
                            spanned over 15 years.
                            Driven by an insatiable curiosity to explore the beauty in everyday moments, Damien has
                            honed her craft meticulously. Her background in digital media provided her with a solid
                            foundation, but it's her keen eye for detail and an innate ability to capture raw emotions
                            that truly set her apart.
                            Damien's journey is more than just taking pictures; it's about capturing the essence of the
                            human spirit, the fleeting magic of nature, and the emotions that define our lives. With
                            each click of her camera, she weaves stories that transcend time and space.</div>
                    </div>
                </div>
            </div>
        </div>
        <div class="section2">
            <div class="top">
                <div class="top-title">
                    <div class="subtitle">Journey</div>
                    <h1>Damien's Journey - A Timeline</h1>
                </div>
            </div>
            <div class="bottom">
                <div class="container">
                    <div class="sub-container">
                        <div class="year">Year - 2005</div>
                        <div class="text">In 2005, Damien acquired her first camera, igniting her passion for
                            photography. She started experimenting with landscapes and candid shots, marking the
                            beginning of her visual storytelling journey.</div>
                    </div>
                    <div class="sub-container">
                        <div class="year">Year - 2010</div>
                        <div class="text">Damien pursued a degree in Fine Arts with a focus on photography, refining her
                            technical skills and artistic sensibilities.</div>
                    </div>
                </div>
                <div class="container">
                    <div class="sub-container">
                        <div class="year">Year - 2012</div>
                        <div class="text">In 2012, Damien held her first solo exhibition, showcasing her unique
                            perspective on nature and people through her lens.</div>
                    </div>
                    <div class="sub-container">
                        <div class="year">Year - 2015</div>
                        <div class="text">Damien officially launched her photography business in 2015, offering
                            portrait, event, and commercial photography services.</div>
                    </div>
                </div>
                <div class="container">
                    <div class="sub-container">
                        <div class="year">Year - 2017</div>
                        <div class="text">Damien's work took her beyond the USA, capturing breathtaking scenes and
                            cultures from around the world.</div>
                    </div>
                    <div class="sub-container">
                        <div class="year">Year - 2020</div>
                        <div class="text">In 2020, Damien's dedication and creativity earned her several prestigious
                            photography awards, solidifying her position as a visionary photographer.</div>
                    </div>
                </div>
            </div>
        </div>

        <div class="section3">
            <div class="top">
                <div class="top-title">
                    <div class="subtitle">Testimonials</div>
                    <h1>What My Clients Say</h1>
                </div>
            </div>
            <div class="top">
                <div class="top-title">
                    <div class="text">Total Reviews</div>
                    <div class="number">323</div>
                </div>
                <div class="btn-container">
                    <div class="small-btn-container">
                        <img class="arrow-left-btn" @click="previousReview" src="~assets/image/arrow-left.svg">
                        <img class="arrow-right-btn" @click="nextReview" src="~assets/image/arrow-right.svg">
                    </div>
                    <nuxt-link to="/portfolio-page">
                        <div class="testimonial-btn">View All Testimonials -></div>
                    </nuxt-link>
                </div>
            </div>
            <div class="bottom">
                <div class="review-item" v-for="(review, index) in client_reviews" :key="index"
                    v-show="index >= activeSlide && index < activeSlide + 3">
                    <div class="header">
                        <div class="header-text">
                            <div class="header-name">{{ review.name }}</div>
                            <div class="header-place">{{ review.place }}</div>
                        </div>
                        <div class="logo-wrapper">
                            <img class="logo" src="~assets/image/facebook.png" />
                            <img class="logo" src="~assets/image/twitter.png" />
                            <img class="logo" src="~assets/image/linkedin.png" />
                        </div>
                    </div>
                    <div class="star-container">
                        <img class="star-yellow" src="~assets/image/star-yellow.svg">
                        <img class="star-yellow" src="~assets/image/star-yellow.svg">
                        <img class="star-yellow" src="~assets/image/star-yellow.svg">
                        <img class="star-yellow" src="~assets/image/star-yellow.svg">
                        <img class="star-yellow" src="~assets/image/star-yellow.svg">
                    </div>
                    <div class="body">{{ review.text }}</div>
                </div>
            </div>

        </div>
    </div>
</template>
<script>
export default {
    data() {
        return {
            client_reviews: [
                {
                    name: 'Emily Johnson',
                    place: 'USA, California',
                    text: 'Damien\'s photography doesn\'t just capture moments; it captures emotions. Hes work is simply mesmerizing.'

                },
                {
                    name: 'John Smith',
                    place: 'USA, California',
                    text: 'Damien has an incredible talent for making every event feel effortless, and the results speak for themselves.'

                },
                {
                    name: 'Samantha Davis',
                    place: 'USA, California',
                    text: 'I was blown away by Damien\'s ability to capture the essence of our wedding day. Hes photographs are our cherished memories.'

                },
                {
                    name: 'Amy Chan',
                    place: 'USA, California',
                    text: 'Nice service.'

                },

            ],
            activeSlide: 0
        };
    },
    methods: {
        previousReview() {
            if (this.activeSlide > 0) {
                this.activeSlide--;
            }
        },

        nextReview() {
            if (this.activeSlide + 3 < this.client_reviews.length) {
                this.activeSlide++;
            }
        }
    }
};

</script>

<style>
.about-me-page {
    width: 100%;
    padding-bottom: 150px;
}

.about-me-page a {
    -webkit-text-decoration: none;
    text-decoration: none;
    color: white;
    cursor: pointer;
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
    align-items: flex-start;
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

.about-me-page .section1 .bottom {
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

.about-me-page .section1 .bottom .title {
    color: var(--Grey-50, #797C86);
    font-size: 34px;
    font-weight: 600;
    text-transform: uppercase;
}



.about-me-page .section2 {
    display: flex;
    width: 1279px;
    flex-direction: column;
    align-items: flex-start;
    padding-top: 350px;
    margin: 150px auto 0 auto;

}

.about-me-page .section2 .bottom {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    gap: 20px;
    align-self: stretch;
    margin-top: 100px;
}

.about-me-page .section2 .container {
    display: flex;
    align-items: flex-start;
    gap: 20px;
    align-self: stretch;
}

.about-me-page .section2 .sub-container {
    display: flex;
    padding: 40px;
    flex-direction: column;
    align-items: flex-start;
    gap: 14px;
    flex: 1 0 0;
}

.about-me-page .section2 .year {
    color: var(--Grey-50, #797C86);
    font-size: 34px;
}

.about-me-page .section2 .text {
    color: var(--Grey-50, #797C86);
}

.about-me-page .section3 {
    display: flex;
    width: 1265px;
    flex-direction: column;
    align-items: flex-start;
    margin: 150px auto 0 auto;
}

.about-me-page .section2 .top,
.about-me-page .section3 .top {
    display: flex;
    align-items: center;
    align-self: stretch;
    justify-content: space-between;

}

.about-me-page .section2 .bottom,
.about-me-page .section3 .bottom {
    display: flex;
    gap: 20px;
    margin-top: 100px;
    width: 1265px;
    overflow: hidden;
}

.about-me-page .section3 .review-item {
    display: flex;
    flex: 0 0 33.33%;
    padding: 30px;
    flex-direction: column;
    align-items: flex-start;
    gap: 24px;
    border-radius: 10px;
    border: 1px solid var(--Dark-12, #1C1C21);
    background: var(--Dark-06, #0E0E10);
    max-width: 346.333px;
}

.about-me-page .section3 .review-item .header {
    display: flex;
    justify-content: space-between;
}

.about-me-page .section3 .review-item .header-name {
    color: var(--Grey-90, #E4E4E6);
    font-family: Manrope;
    font-size: 18px;
}


.about-me-page .review-item .header-place {
    color: var(--Grey-40, #62646C);
}

.about-me-page .review-item .star-yellow {
    width: 20px;
    height: 20px;
}

.about-me-page .review-item .body {
    font-size: 18px;
}

.about-me-page .section2 .subtitle,
.about-me-page .section3 .subtitle {
    color: var(--Grey-50, #797C86);
    font-size: 16px;
    font-weight: 600;
    line-height: normal;
    text-transform: uppercase;
}

.about-me-page .section3 .testimonial-btn {
    display: flex;
    padding: 14px 20px;
    align-items: center;
    border-radius: 8px;
    border: 1px solid #2F2F37;
    background: var(--Dark-12, #1C1C21);
    font-size: 14px;
}

.about-me-page .section3 .top .btn-container {
    display: flex;
    align-items: center;
    gap: 20px;
    align-self: stretch;
}

.about-me-page .section3 .top .small-btn-container {
    display: flex;
    padding: 8px;
    justify-content: flex-end;
    align-items: center;
    gap: 12px;
    border-radius: 100px;
    border: 1px solid var(--Dark-12, #1C1C21);
    background: var(--Dark-03, #070708);
}

.about-me-page .section3 .arrow-left-btn,
.about-me-page .section3 .arrow-right-btn {
    display: flex;
    padding: 10px;
    align-items: center;
    border-radius: 100px;
    border: 1px solid #2F2F37;
    background: var(--Dark-12, #1C1C21);
    width: 28px;
    height: 28px;
}

.about-me-page .logo-wrapper {
    display: flex;
    padding: 8px;
    justify-content: flex-end;
    align-items: center;
    gap: 10px;
}

.about-me-page .logo {
    width: 16px;
    height: 16px;
    display: flex;
    padding: 12px;
    align-items: center;
    border-radius: 100px;
    border: 1px solid #2F2F37;
    background: var(--Dark-12, #1C1C21);
}
</style>