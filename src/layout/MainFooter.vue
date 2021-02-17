<template>
  <footer
    class="footer"
    :class="{ [`footer-${type}`]: type }"
    :data-background-color="backgroundColor"
  >
    <div class="container">
      <nav>
        <ul>
          <li>
            <a href="https://www.creative-tim.com">
              Stéphane Zayat
            </a>
          </li>
          <li>
            <a href="https:///presentation.creative-tim.com">
              En savoir plus
            </a>
          </li>
          <li>
            <a href="https:///blog.creative-tim.com">
              MyFootball
            </a>
          </li>
          <li>
            <a href="https://www.creative-tim.com/license">
             licences
            </a>
          </li>
        </ul>
      </nav>
      <div class="copyright">
        &copy; {{ year }}, Crée <md-icon>favorite</md-icon> par
        <a href="https://www.creative-tim.com/" target="_blank">Stéphane Zayat</a>
      
      </div>
    </div>
  </footer>
</template>
<script>
export default {
  props: {
    backgroundColor: String,
    type: String
  },
  data() {
    return {
      year: new Date().getFullYear()
    };
  }
};
</script>
<style></style>
