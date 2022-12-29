<template>
  <div></div>
    <div class="modal-dialog">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title">Modal title</h5>
        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
      </div>
      <div class="modal-body">
        <p>Modal body text goes here.</p>
      </div>
      <div class="modal-footer">
        <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
        <button type="button" class="btn btn-primary">Save changes</button>
      </div>
    </div>
  </div>
</template>

<script>
export default{}
</script>

<style>
.modal{
    position: fixed;
    top: 0;
    left: 0;
    z-index: var(--bs-modal-zindex);
    display: block;
    width: 100%;
    height: 100%;
    overflow-x: hidden;
    overflow-y: auto;
    outline: 0;
  }

  .modal.show .modal-dialog {
    transform: none;
}

.modal.fade .modal-dialog {
    transition: transform .3s ease-out;
    transform: translate(0,-50px);
}

.modal-dialog {
    position: relative;
    width: auto;
    margin: var(--bs-modal-margin);
    pointer-events: none;
}

.modal-content {
    position: relative;
    display: flex;
    flex-direction: column;
    width: 100%;
    color: var(--bs-modal-color);
    pointer-events: auto;
    background-color: var(--bs-modal-bg);
    background-clip: padding-box;
    border: var(--bs-modal-border-width) solid var(--bs-modal-border-color);
    border-radius: var(--bs-modal-border-radius);
    outline: 0;
}
</style>