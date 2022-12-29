<template>
  <div class="modal"></div>
    <div class="modal-dialog">
    <div class="modal-content">
      <div class="modal-header">
        <h1 class="modal-title">{{ title }}</h5>
        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
      </div>
      <div class="modal-body">
        <p>Modal body text goes here.</p>
      </div>
    </div>
  </div>
</template>

<script>
export default{
  props:{
    title:{
      type:String,
      required: true
    },
    content:{
      type:String,
      required: true
    },
  },

}
</script>

<style scoped lang="css">
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
    background-color: rgba(0, 0,0, 0.2);
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
    background-color: white;
}

.modal-header {
    display: flex;
    flex-shrink: 0;
    align-items: center;
    justify-content: space-between;
    padding: var(--bs-modal-header-padding);
    border-bottom: var(--bs-modal-header-border-width) solid var(--bs-modal-header-border-color);
    border-top-left-radius: var(--bs-modal-inner-border-radius);
    border-top-right-radius: var(--bs-modal-inner-border-radius);
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