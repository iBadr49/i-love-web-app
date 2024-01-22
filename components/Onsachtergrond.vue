<template>
  <link
    href="https://cdn.jsdelivr.net/npm/boxicons@2.0.5/css/boxicons.min.css"
    rel="stylesheet"
  />

  <div class="container">
    <div class="left-panel">
      <h1>Onze achtergrond</h1>
      <p>
        FDND werkt nauw samen met bedrijven uit de creatieve industrie. Tijdens
        de opleiding doe je veel ervaring op in de praktijk en krijg je ook de
        kans om een netwerk op te bouwen, waarbinnen je mogelijk een stageplek
        en een werkplek kunt vinden. Bij We ♥ Web sessies luisteren we naar
        talks en bespreken we maatschappelijke thema's, vaak met een
        interessante spreker uit de beroepspraktijk.
      </p>
    </div>
    <div class="right-panel">
      <img src="assets/img/about1.jpeg" class="student-img" id="img" />
    </div>
  </div>
</template>

<style scoped>
.container {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 20px;
  margin-top: 20px;
  padding: 2rem;
}

.left-panel,
.right-panel {
  display: flex;
  flex-direction: column;
}

img {
  border-radius: 20px;
  height: 80vh;
}

h1 {
  margin-bottom: 30px;
  /* font-size: 40px; */
}

p {
  font-size: 20px;
  /* color: var(--color-1); */
  line-height: 1.6;
  max-width: 45vw;
}

@media only screen and (max-width: 1024px) {
  img {
    width: 40vw;
    height: 60vh;
  }
}

@media only screen and (max-width: 768px) {
  .container {
    grid-template-columns: repeat(1, 2fr);
  }

  p {
    max-width: none;
  }

  .right-panel {
    display: none;
  }

  .left-panel {
    border: 1px solid var(--color-1);
    border-radius: 20px;
    padding: 10px;
  }
}
</style>
