<template>
  <div class="app" dir="rtl">
    <Navbar />
    <div class="app-body">
      <!-- <Sidebar :navItems="nav" /> -->
      <main class="main">
        <!-- <breadcrumb :list="list" /> -->
        <div class="container-fluid">
          <nuxt />
        </div>
      </main>
      <!-- <AppAside /> -->
    </div>
    <!-- <AppFooter /> -->
  </div>
</template>

<script>
import Navbar from "~/components/Header/Navbar";

export default {
  components: {
    Navbar
  }
};
</script>
