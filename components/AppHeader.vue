<!-- components/AppHeader.vue -->
<template>
  <header class="header">
    <div class="header-left">
      <p>
        i
        <svg
          xmlns="http://www.w3.org/2000/svg"
          height="18"
          width="18"
          viewBox="0 0 512 512"
        >
          <path
            d="M225.8 468.2l-2.5-2.3L48.1 303.2C17.4 274.7 0 234.7 0 192.8v-3.3c0-70.4 50-130.8 119.2-144C158.6 37.9 198.9 47 231 69.6c9 6.4 17.4 13.8 25 22.3c4.2-4.8 8.7-9.2 13.5-13.3c3.7-3.2 7.5-6.2 11.5-9c0 0 0 0 0 0C313.1 47 353.4 37.9 392.8 45.4C462 58.6 512 119.1 512 189.5v3.3c0 41.9-17.4 81.9-48.1 110.4L288.7 465.9l-2.5 2.3c-8.2 7.6-19 11.9-30.2 11.9s-22-4.2-30.2-11.9zM239.1 145c-.4-.3-.7-.7-1-1.1l-17.8-20c0 0-.1-.1-.1-.1c0 0 0 0 0 0c-23.1-25.9-58-37.7-92-31.2C81.6 101.5 48 142.1 48 189.5v3.3c0 28.5 11.9 55.8 32.8 75.2L256 430.7 431.2 268c20.9-19.4 32.8-46.7 32.8-75.2v-3.3c0-47.3-33.6-88-80.1-96.9c-34-6.5-69 5.4-92 31.2c0 0 0 0-.1 .1s0 0-.1 .1l-17.8 20c-.3 .4-.7 .7-1 1.1c-4.5 4.5-10.6 7-16.9 7s-12.4-2.5-16.9-7z"
          />
        </svg>
        Web
      </p>
    </div>
    <nav class="header-right">
      <ul>
        <!-- <li><a href="#">About me</a></li>
        <li><a href="#">Contact</a></li> -->
        <li aria-label="after">
          <a href="/about">About</a>
        </li>
        <li aria-label="after">
          <a href="/contact">Contact</a>
        </li>
      </ul>
    </nav>
  </header>
</template>

<style scoped>
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 2rem;
  box-shadow: 0 1px 1px rgba(0, 0, 0, 0.075);
}

.header-left p {
  font-weight: bold;
  font-size: 1.5rem;
}

.header-left .svg {
  color: var(--color-1);
}

.header-right ul {
  list-style: none;
  margin: 0;
  padding: 0;
  display: flex;
}

.header-right li {
  margin-right: 1rem;
}

[aria-label="after"] a {
  color: black;
  position: relative;
  text-decoration: none;
  outline: none;
}

[aria-label="after"] a::after {
  content: "";
  position: absolute;
  top: 100%;
  left: 0;
  right: 0;
  height: 0.17em;
  background-color: var(--color-1);
  scale: 0 1;
  transform-origin: right center;
  transition: scale 0.3s;
}

[aria-label="after"] a:hover:after,
[aria-label="after"] a:focus-visible:after {
  scale: 1 1;
  transform-origin: left center;
}

/* .header-right a {
  text-decoration: none;
  color: black;
}
.header-right a:hover {
  color: var(--color-1);
  transition: color 0.3s ease;
} */

@media only screen and (max-width: 600px) {
  .header {
    flex-direction: column;
    text-align: center;
  }

  .header-left p {
    margin-bottom: 1rem;
  }

  .header-right ul {
    margin-top: 1rem;
  }

  .header-right li {
    margin-right: 10px;
    margin-left: 10px;
  }
}
</style>
