<template>
  <div class="hero-biography-body">
<h2>Biography</h2>
            <!-- Button trigger modal -->
<button type="button" class="btn btn-info" data-toggle="modal" data-target="#HeroBiography">
  Learn More
</button>

<!-- Modal -->
<div class="modal fade" id="HeroBiography" tabindex="-2" role="dialog" aria-labelledby="HeroBiographyTitle" aria-hidden="true">
  <div class="modal-dialog modal-dialog-centered" role="document">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title" id="HeroBiography">Biography</h5>
        <button type="button" class="close" data-dismiss="modal" aria-label="Close">
          <span aria-hidden="true">&times;</span>
        </button>
      </div>
      <div class="modal-body">
        <p><span>Aliases:</span> {{ aliases }}</p>
        <p><span>Alignment:</span> {{ alignment }}</p>
        <p><span>Alter-Egos</span>:{{ alterEgos }}</p>
        <p><span>First Appearance:</span> {{ firstAppearance }}</p>
        <p><span>Full Name:</span> {{ fullName }}</p>
        <p><span>Gender:</span> {{ gender }}</p>
        <p><span>Place Of Birth:</span> {{ placeOfBirth }}</p>
        <p><span>Publisher:</span> {{ publisher }}</p>
      </div>
      <div class="modal-footer">
        <button type="button" class="btn btn-secondary" data-dismiss="modal">Close</button>
      </div>
    </div>
  </div>
</div>
  </div>
</template>


<script>
export default {
  name: 'HeroBiography',
  props: {
      aliases: Array,
      alignment: String,
      alterEgos: String,
      firstAppearance: String,
      fullName: String,
      gender: String,
      placeOfBirth: String,
      publisher: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

/* MODAL POPUP STYLING */
.modal-content .modal-body span {
  font-weight: bold;
}

.modal-content {
  color: #293C4E;
}
</style>
