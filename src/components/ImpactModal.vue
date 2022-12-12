<template>
  <div class="modal fade" id="impactModal" tabindex="-1" aria-labelledby="impactModalLabel" aria-hidden="true">
    <div class="modal-dialog modal-xl modal-dialog-centered">
      <div class="modal-content">
        <div class="modal-header">
          <h1 class="modal-title fs-5" id="impactModalLabel">The brand's impact on the industry</h1>
          <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
        </div>
        <div class="modal-body">
          <div style="display: flex; flex-direction: row; align-items: center;">
            <img src="../assets/crystalmask.gif" style="margin: 15px; height: 400px; width: 400px;">
            <p style="font-size: 1.3em;">{{impact_info.description}}</p>
          </div>
          <small><a href="https://www.aphrodite1994.com/blog/index.php/maison-margiela-brand-guide" target="_blank">Source</a></small>
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
    name: "ImpactModal",
    props: ["impact_info"]
    
}
</script>

<style scoped>
</style>