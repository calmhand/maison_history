<template>
    <div id="carouselExampleControls" class="carousel carousel-dark slide" data-bs-ride="carousel">
        <div class="carousel-inner">
            <div class="carousel-item active">
                <iframe height="400px" width="700px" :src="showsList[0]"></iframe>
            </div>
            <div class="carousel-item">
                <iframe height="400px" width="700px" :src="showsList[1]"></iframe>
            </div>
            <div class="carousel-item">
                <iframe height="400px" width="700px" :src="showsList[2]"></iframe>
            </div>
            <div class="carousel-item">
                <iframe height="400px" width="700px" :src="showsList[3]"></iframe>
            </div>
            <div class="carousel-item">
                <iframe height="400px" width="700px" :src="showsList[4]"></iframe>
            </div>
        </div>
        <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleControls" data-bs-slide="prev">
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Previous</span>
        </button>
        <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleControls" data-bs-slide="next">
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Next</span>
        </button>
    </div>
</template>

<script>
export default {
    name: "ShowsCarousel",
    props: ["showsList"]
}
</script>

<style scoped>
    video {
        width: 1000px;
    }
</style>