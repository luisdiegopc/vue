<template>
  <div class="container mt-12" style="border-radius: 10px; border: solid 2px red;">
      <button
        type="button"
        class="btn btn-primary"
        data-bs-toggle="modal"
        data-bs-target="#exampleModal"
      >
        Abrir Modal
      </button>
  
      <div class="modal fade" id="exampleModal" tabindex="-1" aria-hidden="true">
        <div class="modal-dialog">
          <div class="modal-content">
            <div class="modal-header">
              <h5 class="modal-title">Modal funcionando!</h5>
              <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
            </div>
            <div class="modal-body">Bootstrap foi instalado com sucesso!OOOOOO</div>
          </div>
        </div>
      </div>
    </div>    
</template>
 
<script>
export default {
  name: "ExBootstrap",
};
</script>