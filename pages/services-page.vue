<template>
    <div class="services-page">
        <div class="section1">
            <div class="background">
                <img class="background-pic" src="~assets/image/services-page.png">
                <div class="overlay">
                    <div class="section1-left">
                        <div class="section1-text">About</div>
                        <h1 class="section1-heading">Damien Braun</h1>
                    </div>

                    <div class="bottom-pic">
                        <img class="star" src="~assets/image/star-with-circle.svg">
                        <div class="text">Scroll Down To See My Journey</div>
                    </div>
                </div>
            </div>
        </div>
        <div id="Events" class="events-section"></div>
    </div>


    
</template>

<style>
.services-page {
    width: 100%;
    padding-bottom: 150px;
}

.services-page a {
    -webkit-text-decoration: none;
    text-decoration: none;
    color: white;
    cursor: pointer;
}

.services-page .section1 {
    display: flex;
    padding: 0 80px;
    align-items: center;
    height: 100%;
    position: relative;
    margin-top: 80px;

}

.services-page .section1-left {
    margin-bottom: 24px;
}

.services-page .section1-text {
    color: var(--Grey-40, #62646C);
    font-size: 18px;
    font-weight: 600;
    line-height: normal;
    font-style: normal;
    text-transform: uppercase;
}

.services-page .section1-heading {
    font-size: 48px;
}

.services-page .section1 .background {
    position: relative;
    z-index: 1;
}

.services-page .section1 .background-pic {
    height: 100%;
    width: 100%;
}

.services-page .section1 .overlay {
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


</style>
<script>
export default {
    mounted() {
        this.scrollToSection();
    },
    methods: {
        scrollToSection() {
            const hash = this.$route.hash;
            if (hash) {
                const element = document.getElementById(hash.substr(1));
                if (element) {
                    element.scrollIntoView({ behavior: 'smooth' })
                }
            }
        }
    },
    watch: {
        '$route'() {
            this.scrollToSection();
        }
    }
}
</script>