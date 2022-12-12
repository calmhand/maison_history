<template>
    <div id="home-page">
        <video autoplay muted loop id="myVideo">
            <source src="./assets/runway.mp4" type="video/mp4">
        </video>
        <div id="component-container">
            <BrandGrid />
            <NavBar />
        </div>
        <a href="https://github.com/calmhand/maison_history#readme" target="_blank">readme</a>
    </div>
</template>

<script>
import BrandGrid from './components/BrandGrid.vue'
import NavBar from './components/NavBar.vue'

export default {
    name: "Home",
    components: { NavBar, BrandGrid },
}
</script>

<style scoped>
    #home-page {
        height: 100%;
        display: flex;
        flex-direction: column;
    }

    #component-container {
        margin-top: 1000px 0;
    }

</style>