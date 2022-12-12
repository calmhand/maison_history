<template>
  <div class="modal fade" id="creditsModal" tabindex="-1" aria-labelledby="creditsModalLabel" aria-hidden="true">
    <div class="modal-dialog modal-xl modal-dialog-centered">
      <div class="modal-content">
        <div class="modal-header">
          <h1 class="modal-title fs-5" id="creditsModalLabel">Credits</h1>
          <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
        </div>
        <div class="modal-body">
          <h3>Site created by Johnny Goulbourne for NMIX 4050 Final Project</h3>
          <small>This site uses Vue CLI and Bootstrap 5.</small>
          <small>This site is a small introduction to the world famous fashion house Maison Margiela.</small>
          <small><a>source code</a></small>
          <!-- TODO: LINK TO GITHUB -->
          <h4>Images retrieved from Google Images</h4>
          <h4 style="text-decoration: underline;">Sources</h4>
          <a href="https://www.aphrodite1994.com/blog/index.php/maison-margiela-brand-guide">aphrodite1994</a><br>
          <a href="https://www.coggles.com/life/fashion/maison-margiela-fashion-history/">coggles</a>
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
    name: "CreditsModal",
    
}
</script>

<style scoped>
</style>