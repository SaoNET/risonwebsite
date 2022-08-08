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
            <a href="/">
              Webaplant
            </a>
          </li>
          <li>
            <a href="/aboutus">
              About Us
            </a>
          </li>
          <li>
            <a href="#">
              Blog
            </a>
          </li>
          <li>
            <a href="#">
              Licenses
            </a>
          </li>
          
          <li>
            <a href="https://twitter.com/Webaplant" target="_blank">
              <i class="fab fa-twitter"></i>
              <p class="hidden-lg">Twitter</p>
              <md-tooltip md-direction="bottom">Follow us on Twitter</md-tooltip>
            </a>
          </li>
          <li>
            <a href="https://www.facebook.com/Webaplant" target="_blank">
              <i class="fab fa-facebook-square"></i>
              <p class="hidden-lg">Facebook</p>
              <md-tooltip md-direction="bottom">Like us on Facebook</md-tooltip>
            </a>
          </li>
          <li>
            <a href="https://www.instagram.com/Webaplant" target="_blank">
              <i class="fab fa-instagram"></i>
              <p class="hidden-lg">Instagram</p>
              <md-tooltip md-direction="bottom">Follow us on Instagram</md-tooltip>
            </a>
          </li>
        </ul>
      </nav>
      <div class="copyright">
        &copy; {{ year }}, made with <md-icon>favorite</md-icon> by
        <a href="/" target="_blank">Webaplant</a>.
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
