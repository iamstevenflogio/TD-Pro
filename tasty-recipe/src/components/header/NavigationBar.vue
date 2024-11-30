<script setup>
import { onBeforeMount, onMounted, onBeforeUpdate, onUpdated, onBeforeUnmount, onUnmounted, onErrorCaptured } from 'vue';
import SearchMenu from './SearchMenu.vue';
import SignUpMenu from './SignupMenu.vue';

// Lifecycle Hooks
onBeforeMount(() => {
  console.log('Navbar component is about to be mounted');
});

onMounted(() => {
  console.log('Navbar component has been mounted');
});

onBeforeUpdate(() => {
  console.log('Navbar component is about to update');
});

onUpdated(() => {
  console.log('Navbar component has been updated');
});

onBeforeUnmount(() => {
  console.log('Navbar component is about to be unmounted');
});

onUnmounted(() => {
  console.log('Navbar component has been unmounted');
});

onErrorCaptured((err, instance, info) => {
  console.error('Error captured in Navbar:', err, instance, info);
  return false; // Return false to stop the propagation of the error
});
</script>



<template>
    <div
    class="header__navbar row
    justify-content-between align-items-center"
    style="width: 450px"
    >
    <!-- Component SearchMenu -->
     <SearchMenu />
    <!-- Component SignupMenu -->
     <SignupMenu />
    </div>
</template>