<template>
  <b-navbar class="navbar-custom">
    <template #brand>
      <b-navbar-item tag="router-link" :to="{ path: '/' }">
        <img
          src="@/assets/images/v-logo.svg"
          alt="Lightweight UI components for Vue.js based on Bulma"
          class="brand-logo ml-6"
        />
      </b-navbar-item>
    </template>
    <template #start> </template>

    <template #end>
      <b-navbar-item tag="div">
        <div class="buttons">
          <a href="https://x.com/varemoney" target="_blank" class="icon-link twit-navlink">
            <font-awesome-icon :icon="['fab', 'x-twitter']" class="fa-icon" />
          </a>
          <a href="https://t.me/varemoney" target="_blank" class="icon-link tel-navlink">
            <font-awesome-icon :icon="['fab', 'telegram']" class="fa-icon" />
          </a>
        </div>
      </b-navbar-item>
    </template>
  </b-navbar>
</template>

<style scoped>
.navbar-custom {
  position: relative;
  z-index: 10; /* Ensure navbar is above the hero image */
}

.brand-logo {
  min-height: 256px; /* Set the minimum height of the logo */
}

.icon-link {
  color: #e0ff00; /* Set the color of the icons */
  transition: color 0.3s ease;
}

.icon-link:hover {
  color: darken(#e0ff00, 20%); /* Darker color on hover */
}

.fa-icon {
  height: 64px; /* Set the height of the icons */
  width: 64px; /* Set the width of the icons */
}

.tel-navlink {
  position: absolute;
  top: 25px;
  right: 25px;
}

.twit-navlink {
  position: absolute;
  top: 25px;
  right: 75px;
}
</style>
