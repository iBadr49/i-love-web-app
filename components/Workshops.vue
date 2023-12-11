<!-- components/Workshop.vue -->
<template>
<div class="container">
    <div class="card-container">
        <article class="card-article">
            <img src="assets/img/accessibility.png" class="card-img">
            <div class="card-data">
                <span class="card-description"> Cyd | 23 dec 2023</span>
                <h2 class="card-title">workshop 1</h2>
                <a href="#" class="card-button">Read more</a>
            </div>
        </article>

        <article class="card-article">
            <img src="assets/img/accessibility.png" class="card-img">
            <div class="card-data">
                <span class="card-description"> Joost | 24 oct 2023</span>
                <h2 class="card-title">workshop 2</h2>
                <a href="#" class="card-button">Read more</a>
            </div>
        </article>

        <article class="card-article">
            <img src="assets/img/accessibility.png" class="card-img">
            <div class="card-data">
                <span class="card-description">Koop | 23 dec 2023</span>
                <h2 class="card-title">workshop 3</h2>
                <a href="#" class="card-button">Read more</a>
            </div>
        </article>
        <article class="card-article">
            <img src="assets/img/accessibility.png" class="card-img">
            <div class="card-data">
                <span class="card-description">Koop | 23 dec 2023</span>
                <h2 class="card-title">workshop 4</h2>
                <a href="#" class="card-button">Read more</a>
            </div>
        </article>

        <article class="card-article">
            <img src="assets/img/accessibility.png" class="card-img">
            <div class="card-data">
                <span class="card-description">Koop | 23 dec 2023</span>
                <h2 class="card-title">workshop 5</h2>
                <a href="#" class="card-button">Read more</a>
            </div>
        </article>

        <article class="card-article">
            <img src="assets/img/accessibility.png" class="card-img">
            <div class="card-data">
                <span class="card-description">Koop | 23 dec 2023</span>
                <h2 class="card-title">workshop 6</h2>
                <a href="#" class="card-button">Read more</a>
            </div>
        </article>
    </div>
</div>
</template>
  
<style scoped>

.container {
  display: grid;
  place-items: center;
  margin-inline: 1.5rem;
  padding-block: 5rem;
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
  width: 328px;
  border-radius: 1.5rem;
}

.card-data {
  width: 250px;
  background-color: rgb(222, 222, 222);
  padding: 1.5rem 2rem;
  box-shadow: 0 8px 24px hsla(0, 0%, 0%, .15);
  border-radius: 1rem;
  position: absolute;
  bottom: -9rem;
  left: 0;
  right: 0;
  margin-inline: auto;
  opacity: 0;
  transition: opacity 1s 1s;
}

.card-description {
  display: block;
  font-size: small;
  margin-bottom: .25rem;
}

.card-title {
  margin-bottom: .75rem;
}

.card-button {
  text-decoration: none;
  font-size: small;
  color: rgb(0, 123, 254);
}

.card-button:hover {
  text-decoration: underline;
}

.card-article:hover .card-data {
  animation: show-data 1s forwards;
  opacity: 1;
  transition: opacity .3s;
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

@media screen and (min-width: 340px){
  .container{
    margin-inline: 1rem;
  }

  .card-data{
    width: 250px;
    padding: 1rem;
  }
}

@media screen and (min-width: 768px){
  .card-container{
    grid-template-columns: repeat(2, 1fr);
    column-gap: 1.5rem;
  }

}

@media screen and (min-width: 1120px){
  .container{
    height: 100vh;
  }
  .card-container{
    grid-template-columns: repeat(3, 1fr);
  }
  .card-img {
    width: 348px;
  }

}

</style>
  