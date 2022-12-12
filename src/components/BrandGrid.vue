<template>
    <div id="img-container">
        <img id="margiela-logo" src="../assets/Maison_Margiela_logo.png">
    </div>
    <small style="margin: 10px 0;"><strong><i>"fashion is an artistic expression rather than a cult for personality"</i></strong></small>
    <div id="panels-container">
        <Panel class="category-option panel-element" id="artisan-panel" :labelID="0" :name="`Artisanal`" :panelName="`artisan-panel`"/>
        <Panel class="category-option panel-element" id="womens-collection-panel" :labelID="1" :name="`Women's Collection`"/>
        <Panel class="panel-element" id="" :labelID="2" :name="``"/>
        <Panel class="category-option panel-element" id="fragrances-panel" :labelID="3" :name="`Fragrances`"/>
        <Panel class="category-option panel-element" id="womens-wardrobe-panel" :labelID="4" :name="`Woman's Garderobe`"/>
        <Panel class="panel-element" id="" :labelID="5" :name="``"/>
        <Panel class="category-option panel-element" id="mm6-panel" :labelID="6" :name="`MM6`"/>
        <Panel class="panel-element" id="" :labelID="7" :name="``"/>
        <Panel class="category-option panel-element" id="eyeware-panel" :labelID="8" :name="`Eyewear`"/>
        <Panel class="panel-element" id="" :labelID="9" :name="``"/>

        <Panel class="category- panel-element" id="mens-collection-panel" :labelID="10" :name="`Men's Collection`"/>
        <Panel class="category-option panel-element" id="accessories-panel" :labelID="11" :name="`Accessories`"/>
        <Panel class="category-option panel-element" id="jewelry-panel" :labelID="12" :name="`Jewelry`"/>
        <Panel class="category-option panel-element" id="objects-panel" :labelID="13" :name="`Objects and Catalogs`"/>
        <Panel class="category-option panel-element" id="men-wardrobe-panel" :labelID="14" :name="`Men's Wardrobe`"/>
        <Panel class="panel-element" id="" :labelID="15" :name="``"/>
        <Panel class="panel-element" id="" :labelID="16" :name="``"/>
        
        <Panel class="panel-element" id="" :labelID="17" :name="``"/>
        <Panel class="panel-element" id="" :labelID="18" :name="``"/>
        <Panel class="panel-element" id="" :labelID="19" :name="``"/>
        <Panel class="panel-element" id="" :labelID="20" :name="``"/>
        <Panel class="panel-element" id="" :labelID="21" :name="``"/>
        <Panel class="category-option" id="shoes-panel" :labelID="22" :name="`Shoes`"/>
        <Panel class="panel-element" id="" :labelID="23" :name="``"/>
    </div>
</template>

<script>
import Panel from "./Panel.vue"
import maisonLabels from "../maison.js"


export default {
    name: "BrandGrid",
    components: {Panel},
    data() {
        return {
            labels : maisonLabels,
        }
    },
    methods: {

    }
}
</script>

<style scoped>
    #img-container {
        display: flex;
        justify-content: center;
        margin-top: 500px;
    }

    #margiela-logo {
        height: 100px;
        width: 450px;
        text-align: center;
    }

    .category-option {
        cursor: pointer;
        animation: fade 3s infinite;
    }

    @keyframes fade {
        0% {
            opacity: 1;
        }

        50% {
            opacity: 0.2;
        }

        100% {
            opacity: 1;
        }
    }

    .panel-element {
        margin: 0 10px;
    }

    #panels-container {
        display: flex;
        flex-direction: row;
        justify-content: center;
        align-items: left;
        align-content: center;
        flex-wrap: wrap;
        margin: 10px;
    }

    Panel {
        margin: 10px 0;
    }
    
</style>