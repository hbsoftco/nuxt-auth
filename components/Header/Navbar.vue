<template>
  <div>
  <b-navbar toggleable="lg" type="dark" variant="info">
    <b-navbar-brand href="#">رویدانا</b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav>
        <b-nav-item href="#">صفحه اصلی</b-nav-item>
        <b-nav-item href="#" disabled></b-nav-item>
      </b-navbar-nav>

      <!-- Right aligned nav items -->
      <b-navbar-nav class="mr-auto">
        <b-nav-form>
          <b-form-input size="sm" class="mr-sm-2" placeholder="جستجو ..."></b-form-input>
          <b-button size="sm" class="my-2 my-sm-0" type="submit">جستجو</b-button>
        </b-nav-form>

        <b-nav-item-dropdown text="زبان" left>
          <b-dropdown-item href="#">EN</b-dropdown-item>
          <b-dropdown-item href="#">ES</b-dropdown-item>
          <b-dropdown-item href="#">RU</b-dropdown-item>
          <b-dropdown-item href="#">FA</b-dropdown-item>
        </b-nav-item-dropdown>

        <b-nav-item-dropdown left>
          <!-- Using 'button-content' slot -->
          <template v-slot:button-content>
            <em>حساب کاربری</em>
          </template>
          <b-dropdown-item href="#">پروفایل</b-dropdown-item>
          <b-dropdown-item href="#">خروج</b-dropdown-item>
        </b-nav-item-dropdown>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
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
