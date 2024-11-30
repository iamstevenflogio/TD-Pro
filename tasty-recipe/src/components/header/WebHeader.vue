<script setup>
import { onBeforeMount, onMounted, onBeforeUpdate, onUpdated, onBeforeUnmount, onUnmounted, onErrorCaptured } from 'vue';
import NavigationBar from './NavigationBar.vue';

// Lifecycle Hooks
onBeforeMount(() => {
  console.log('WebHeader component is about to be mounted');
});

onMounted(() => {
  console.log('WebHeader component has been mounted');
});

onBeforeUpdate(() => {
  console.log('WebHeader component is about to update');
});

onUpdated(() => {
  console.log('WebHeader component has been updated');
});

onBeforeUnmount(() => {
  console.log('WebHeader component is about to be unmounted');
});

onUnmounted(() => {
  console.log('WebHeader component has been unmounted');
});

onErrorCaptured((err, instance, info) => {
  console.error('Error captured in WebHeader:', err, instance, info);
  return false; // Return false to stop the propagation of the error
});
</script>


<template>
    <header
        class="shadow-sm container-fluid
        
        bg-white py-3 border-bottom fixed-top" >
        
        <div class="container-md d-flex
        
        justify-content-between align-items-center" >
        <img src="@/assets/images/Logo.png" alt="Logo" />
        <!-- Component NavigationBar -->
         <NavigationBar />
        </div>
    </header>
</template>