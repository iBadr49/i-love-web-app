
<template>
  <footer class="blog-footer">
    <div class="container">
      <div class="footer-content">
        <div class="footer-links">
          <!-- <router-link to="#">Contact Us</router-link> -->
          <!-- <router-link to="/contact">Contact Us</router-link> -->
        </div>
      </div>
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
.blog-footer {
  justify-content: space-between;
  padding: 2rem;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
}

.footer-content {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.footer-links {
  display: flex;
  gap: 20px;
}

.footer-links a {
  text-decoration: none;
  color: #333;
}

.footer-social {
  margin-top: 20px;
}

.footer-social a {
  margin-right: 15px;
  font-size: 1.5em;
  color: #333;
}

.footer-social i:hover {
  color: var(--color-1);
}
</style>
