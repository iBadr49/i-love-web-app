<!-- components/Workshop.vue -->
<template>
  <div class="container">
    <div class="card-container">
      <article class="card-article">
        <img src="assets/img/image9.jpg" class="card-img" />
        <div class="card-data">
          <span class="card-description"> Tim Borst | 6 oct 2023</span>
          <h2 class="card-title">Freelancen</h2>
          <a href="/freelancen" class="card-button">Read more</a>
        </div>
      </article>

      <article class="card-article">
        <img src="assets/img/image2.jpg" class="card-img" />
        <div class="card-data">
          <span class="card-description"> Ischa Gast | 20 oct 2023</span>
          <h2 class="card-title">Accessibility</h2>
          <a href="/accessibility" class="card-button">Read more</a>
        </div>
      </article>
      
      <article class="card-article">
        <img src="assets/img/image6.jpg" class="card-img" />
        <div class="card-data">
          <span class="card-description"> Fenna de Wilde | 19 jan 2023</span>
          <h2 class="card-title">workshop 3</h2>
          <a href="#" class="card-button">Read more</a>
        </div>
      </article>

      <!-- 

      <article class="card-article">
        <img src="assets/img/image5.jpg" class="card-img" />
        <div class="card-data">
          <span class="card-description">Koop | 23 dec 2023</span>
          <h2 class="card-title">workshop 5</h2>
          <a href="#" class="card-button">Read more</a>
        </div>
      </article>

      <article class="card-article">
        <img src="assets/img/image3.jpg" class="card-img" />
        <div class="card-data">
          <span class="card-description">Koop | 23 dec 2023</span>
          <h2 class="card-title">workshop 6</h2>
          <a href="#" class="card-button">Read more</a>
        </div>
      </article>

      <article class="card-article">
        <img src="assets/img/image10.jpg" class="card-img" />
        <div class="card-data">
          <span class="card-description"> Joost | 24 oct 2023</span>
          <h2 class="card-title">workshop 7</h2>
          <a href="#" class="card-button">Read more</a>
        </div>
      </article> -->
    </div>
  </div>
</template>

<style scoped>
.container {
  display: grid;
  place-items: center;
  margin-inline: 1.5rem;
  padding-block: 5rem;
  animation: grow 1s;
}

@keyframes grow {
  0% {
    transform: scale(0.2);
  }
  100% {
    transform: scale(1);
  }
}

.card-container {
  display: grid;
  row-gap: 3.5rem;
}

.card-article {
  position: relative;
  overflow: hidden;
}

.card-img {
  width: 330px;
  border-radius: 1.5rem;
  /* border: 1px solid var(--color-1); */
  /* box-shadow: 0 1px var(--color-1); */
}

.card-data {
  width: 250px;
  background-color: whitesmoke;
  padding: 1.5rem 2rem;
  box-shadow: 0 8px 24px hsla(0, 0%, 0%, 0.15);
  border-radius: 1rem;
  position: absolute;
  bottom: -9rem;
  left: 0;
  right: 0;
  margin-inline: auto;
  opacity: 0;
  transition: opacity 1s;
}

.card-description {
  display: block;
  font-size: small;
  margin-bottom: 0.25rem;
}

.card-title {
  margin-bottom: 0.75rem;
}

.card-button {
  text-decoration: none;
  font-size: small;
  color: var(--color-1);
}

.card-button:hover {
  text-decoration: underline;
}

.card-article:hover .card-data {
  animation: show-data 1s forwards;
  opacity: 1;
  transition: opacity 0.3s;
}

.card-article:hover {
  animation: remove-overflow 2s forwards;
}

.card-article:not(:hover) {
  animation: show-overflow 2s forwards;
}

.card-article:not(:hover) .card-data {
  animation: remove-data 1s forwards;
}

@keyframes show-data {
  50% {
    transform: translateY(-10rem);
  }
  100% {
    transform: translateY(-7rem);
  }
}

@keyframes remove-overflow {
  to {
    overflow: initial;
    transform: translateY(0rem);
  }
}

@keyframes show-overflow {
  0% {
    overflow: hidden;
    pointer-events: none;
  }
  50% {
    overflow: hidden;
  }
}

@keyframes remove-data {
  to {
    transform: translateY(0);
    opacity: 0;
  }
}

@media screen and (min-width: 340px) {
  .container {
    padding: 1rem;
    margin-inline: 1rem;
  }

  .card-data {
    width: 250px;
    padding: 1rem;
  }
}

@media screen and (min-width: 768px) {
  .card-container {
    grid-template-columns: repeat(2, 1fr);
    column-gap: 1.5rem;
  }
}

@media screen and (min-width: 1120px) {

  .card-container {
    grid-template-columns: repeat(3, 1fr);
  }
  .card-img {
    width: 340px;
  }
}
</style>
