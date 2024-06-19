<template>
    <div class="about-me-page">
        <div class="section1">
            <div class="background">
                <img class="background-pic" src="~assets/image/about-me-page.png">
            </div>
            <div class="overlay">
                <div class="section1-left">
                    <div class="section1-left-text">About</div>
                    <h1 class="section1-heading">Damien Braun</h1>
                </div>
            </div>


        </div>
    </div>
</template>


<script>
</script>

<style>
.about-me-page {
    width: 100%;
    margin-bottom: 200px;
}


.about-me-page .section1 {
    display: flex;
    padding: 0 80px;
    /* justify-content: space-between; */
    align-items: center;
    height: 262px;
}

.about-me-page .section1-left-text {
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
    /* top:278px; */
    /* width: 100%; */
}

.about-me-page .section1 .background-pic {
    height: 784px;
    /* top:278px; */
    /* width: 100%; */
}

.about-me-page .section1 .overlay {
    position: absolute;
}
</style>