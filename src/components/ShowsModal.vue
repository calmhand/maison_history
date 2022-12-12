<template>
  <div class="modal fade" id="showsModal" tabindex="-1" aria-labelledby="showsModalLabel" aria-hidden="true">
    <div class="modal-dialog modal-xl modal-dialog-centered">
      <div class="modal-content">
        <div class="modal-header">
          <h1 class="modal-title fs-5" id="showsModalLabel">Shows</h1>
          <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
        </div>
        <div class="modal-body">
          <ShowsCarousel :showsList="showLinks"/>
        </div>
        <div class="modal-footer">
          <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import ShowsCarousel from "./ShowsCarousel.vue"
export default {
    name: "ShowsModal",
    components: {ShowsCarousel},
    props: ["showLinks"]
}
</script>

<style scoped>
</style>