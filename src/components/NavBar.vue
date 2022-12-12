<template>
    <div id="nav-bar">
        <a @click="displayInfo(`history-modal-btn`)">history</a>
        <a @click="displayInfo(`impact-modal-btn`)">impact</a>
        <a @click="displayInfo(`shows-modal-btn`)">shows</a>
        <a @click="displayInfo(`credits-modal-btn`)">credits</a>
    </div>

    <HistoryModal :history_info="history"/>
    <button id="history-modal-btn" style="display: none;" type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#historyModal"></button>

    <ImpactModal :impact_info="impact"/>
    <button id="impact-modal-btn" style="display: none;" type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#impactModal"></button>

    <ShowsModal :showLinks="shows.shows"/>
    <button id="shows-modal-btn" style="display: none;" type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#showsModal"></button>

    <CreditsModal />
    <button id="credits-modal-btn" style="display: none;" type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#creditsModal"></button>
</template>

<script>
import HistoryModal from './HistoryModal.vue';
import ImpactModal from './ImpactModal.vue';
import ShowsModal from './ShowsModal.vue';
import CreditsModal from './CreditsModal.vue';
import info from '../maison_info.js'

export default {
    name: "NavBar",
    data() {
        return {
            history : info[0],
            impact : info[1],
            shows : info[2],
        }
    },
    components: { HistoryModal, ImpactModal, ShowsModal, CreditsModal },
    methods: {
        displayInfo(opt) {
            document.getElementById(opt).click()
        }
    }
}
</script>

<style scoped>
    #nav-bar {
        display: flex;
        flex-direction: row;
        justify-content: center;
        margin-bottom: 300px;
    }

    a {
        font-size: 1.5em;
        margin: 0 5%;
        cursor: pointer;
        transition: opacity 0.2s ease-in-out;
    }

    a:hover {
        opacity: 0.5;
    }
</style>