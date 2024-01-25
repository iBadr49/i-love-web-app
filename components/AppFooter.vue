<!-- components/AppFooter.vue -->
<template>
  <footer>
    <div class="container">
      <div class="footer-social">
        <a href="#" target="_blank" rel="noopener noreferrer">
          <i class="bx bxl-twitter"></i>
        </a>
        <a href="#" target="_blank" rel="noopener noreferrer">
          <i class="bx bxl-github"></i>
        </a>
        <a href="#" target="_blank" rel="noopener noreferrer">
          <i class="bx bxl-linkedin"></i>
        </a>
      </div>
    </div>
  </footer>
</template>

<style scoped>
.container {
  justify-content: space-between;
  padding: 2rem;
  margin-top: 40px;
  margin: 0 auto;
}

.footer-social {
  margin-top: 20px;
}

.footer-social a {
  margin-right: 15px;
  font-size: 1.5em;
  color: black;
}

.footer-social i:hover {
  color: var(--color-1);
}
</style>
