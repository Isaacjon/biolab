<template>
  <header class="header">
    <nav class="navbar">
      <div class="logo">
        <span>ItLabs</span>
      </div>
      <ul class="menu">
        <li v-for="item in menu_array" :key="item.text">
          <router-link :to="{ name: item.link }">{item.text}</router-link>
        </li>
      </ul>
      <div class="burger"></div>
      <div class="mobile-menu"></div>
      <div class="actions">
        <div class="search">
          <i class="fas fa-search"></i>
        </div>
        <div class="language">
          <span>Eng</span>
          <i class="fas fa-angle-down"></i>

          <span></span>
        </div>
      </div>
    </nav>
  </header>
</template>

<script>
export default {
  data() {
    return {
      menu_array: [
        {
          text: "About us",
          link: "About",
        },
        {
          text: "Catalog",
          link: "Catalog",
        },
        {
          text: "Partners",
          link: "Partners",
        },
        {
          text: "Blog",
          link: "Blog",
        },
        {
          text: "Contact Us",
          link: "Contacts",
        },
      ],
    };
  },
};
</script>

<style lang="scss"></style>
