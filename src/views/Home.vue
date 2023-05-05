<template>
  <div class="row align-items-md-stretch">

    <div class="col-md-6 mb-4">
      <p> located in the South Hero Village</p>
      <p> The oldest artisan cooperative in the Lake Champlain Region</p>
      <!-- <div class="p-5 box border rounded-3 mb-4">
        <h2>Bootstrap Toast</h2>
        <p>Toasts are lightweight notifications designed to mimic the push notifications that have been popularized by mobile and desktop operating systems. They’re built with flexbox, so they’re easy to align and position.</p>

        <button type="button" class="btn btn-outline-secondary" @click="toast.show()">Show Toast</button>
         <div class="position-fixed bottom-0 end-0 p-3 emerge-11">
          <div ref="bsToast" class="toast hide" role="alert" aria-live="assertive" aria-atomic="true">
            <div class="toast-header bg-info text-dark">
              <i class="bi bi-hand-index me-1"></i>
              <strong class="me-auto">Which finger?!</strong>
              <small>Some times ago</small>
              <button type="button" class="btn-close" data-bs-dismiss="toast" aria-label="Close"></button>
            </div>
            <div class="toast-body box">Hello, world! This is a toast message.</div>
          </div>
        </div> -->
      </div>
      <!-- <div class="p-5 box border rounded-3">
        <h2>Bootstrap Grid</h2>
        <p>
          Bootstrap’s grid system uses a series of containers, rows, and columns to layout and align content. It’s built with
          <a href="https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Basic_Concepts_of_Flexbox" target="_blank" rel="noopener noreferrer">flexbox</a>
          and is fully responsive. Below is an example and an in-depth explanation for how the grid system comes together.
        </p>
        <div class="bd-example bd-example-row">
          <div class="row">
            <div class="col-12 col-lg-8">.col-12 .col-lg-8</div>
            <div class="col-12 col-lg-4">.col-12 .col-lg-4</div>
          </div>

          <div class="row">
            <div class="col-6 col-md-4">.col-6 .col-md-4</div>
            <div class="col-6 col-md-4">.col-6 .col-md-4</div>
            <div class="col-12 col-md-4">.col-12 .col-md-4</div>
          </div>

          <div class="row">
            <div class="col-6">.col-6</div>
            <div class="col-6">.col-6</div>
          </div>
        </div>
      </div> -->
      <!-- <div class="p-5 box border rounded-3 mt-4 d-flex justify-content-between">
        <i class="bi bi-house-fill"></i>
        <i class="bi bi-boxes"></i>
        <i class="bi bi-car-front-fill"></i>
        <i class="bi bi-cart4"></i>
        <i class="bi bi-cloud-snow"></i>
        <i class="bi bi-gear"></i>
      </div> -->
    </div>

</template>

<script lang="ts" setup>
import { reactive, onMounted, ref } from "vue";
import { Modal, Toast } from "bootstrap";

defineProps({
  msg: String
});

const state = reactive({ count: 0 });
const modal = ref();
const toast = ref();
const infoModal = ref();
const bsToast = ref();

onMounted(() => {
  modal.value =  new Modal(infoModal.value);
  toast.value = new Toast(bsToast.value);
});
</script>

<style lang="scss" scoped>
#infoModalLabel { color: var(--bs-body-color); }
</style>