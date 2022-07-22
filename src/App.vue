<template>
  <div id="material-kit">
    <!-- <div :class="{ 'nav-open': NavbarStore.showNavbar }"> -->
    <div :class="{ 'nav-open': false }">
      <router-view name="header" />
      <div>
        <router-view />
      </div>
      <router-view name="footer" />
    </div>
  </div>
</template>
