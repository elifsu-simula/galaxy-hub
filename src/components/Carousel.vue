<template>
    <div class="carousel-container">
        <b-carousel
            id="carousel-1"
            v-model="slide"
            :interval="5000"
            controls
            indicators
            background="#ababab"
            img-width="650"
            img-height="450"
            style="text-shadow: 1px 1px 2px #333"
        >
            <!--
            It's important that the images here are 13x9 aspect ratio,
            otherwise the page will jump around when the carousel changes.
            -->
            <a href="https://forms.gle/WKoLb5NUR6FVmeRM9" target="_blank">
                <b-carousel-slide
                    img-src="/images/Scholarships_13x9.png"
                    img-alt="GBCC2025 scholarships available"
                ></b-carousel-slide>
            </a>
            <a href="https://jxtxfoundation.org" target="_blank">
                <b-carousel-slide
                    img-src="/images/jxtx/jxtx-jumbotron.png"
                    img-alt="Donate to the James P. Taylor Foundation for Open Science"
                ></b-carousel-slide>
            </a>
        </b-carousel>
    </div>
</template>

<script>
export default {
    name: "Carousel",
    data() {
        return {
            slide: 0,
        };
    },
};
</script>
<style lang="scss" scoped>
.carousel-container {
    padding-top: 2rem;
    max-width: 650px;
    margin: 0 auto;
}
</style>
