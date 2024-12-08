<script setup>
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";
import Modal from "./components/Modal.vue";
import { store } from "./store/index";
</script>

<template>
  <Header @toggleModal="store.toggleModal(true)" />
  <main class="content">
    <router-view></router-view>
  </main>

  <Modal :isOpen="store.isOpen" @toggleModal="store.toggleModal(false)" />
  <Footer />
</template>

<style scoped></style>
