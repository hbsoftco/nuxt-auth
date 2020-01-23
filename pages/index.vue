<template>
  <div class="animated fadeIn">
    <b-row>
      <b-col md="12">
        <div v-if="$auth.loggedIn">
          {{$auth.user.email}}
          <span>Hossein</span>
        </div>
        <div v-else>
          <span>Please login</span>
        </div>
      </b-col>
    </b-row>
  </div>
</template>

<script>
import Logo from "~/components/Logo.vue";

export default {
  components: {
    Logo
  }
};
</script>

<style></style>
