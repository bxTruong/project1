<template>
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

--bs-modal-zindex: 1055;
    --bs-modal-width: 500px;
    --bs-modal-padding: 1rem;
    --bs-modal-margin: 0.5rem;
    --bs-modal-color: ;
    --bs-modal-bg: var(--bs-body-bg);
    --bs-modal-border-color: var(--bs-border-color-translucent);
    --bs-modal-border-width: var(--bs-border-width);
    --bs-modal-border-radius: var(--bs-border-radius-lg);
    --bs-modal-box-shadow: 0 0.125rem 0.25rem rgba(var(--bs-body-color-rgb), 0.075);
    --bs-modal-inner-border-radius: calc(var(--bs-border-radius-lg) - (var(--bs-border-width)));
    --bs-modal-header-padding-x: 1rem;
    --bs-modal-header-padding-y: 1rem;
    --bs-modal-header-padding: 1rem 1rem;
    --bs-modal-header-border-color: var(--bs-border-color);
    --bs-modal-header-border-width: var(--bs-border-width);
    --bs-modal-title-line-height: 1.5;
    --bs-modal-footer-gap: 0.5rem;
    --bs-modal-footer-bg: ;
    --bs-modal-footer-border-color: var(--bs-border-color);
    --bs-modal-footer-border-width: var(--bs-border-width);
    position: fixed;
    top: 0;
    left: 0;
    z-index: var(--bs-modal-zindex);
    display: none;
    width: 100%;
    height: 100%;
    overflow-x: hidden;
    overflow-y: auto;
    outline: 0;
</style>