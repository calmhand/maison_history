<template>
  <div class="modal fade" id="historyModal" tabindex="-1" aria-labelledby="historyModalLabel" aria-hidden="true">
    <div class="modal-dialog modal-xl modal-dialog-centered">
      <div class="modal-content">
        <div class="modal-header">
          <h1 class="modal-title fs-5" id="historyModalLabel">The History of Maison Margiela</h1>
          <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
        </div>
        <div class="modal-body">
          <div>
            <img src="../assets/maison_numbers.jpg" style="margin: 15px 0;">
            <p style="font-size: 1.3em;">{{history_info.description}}</p>
            <small><a href="https://www.coggles.com/life/fashion/maison-margiela-fashion-history/" target="_blank">Source</a></small>
          </div>
        </div>
        <div class="modal-footer">
          <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
    name: "HistoryModal",
    props: ["history_info"]
    
}
</script>

<style scoped>
</style>