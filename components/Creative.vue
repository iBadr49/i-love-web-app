<!-- components/Creative workshop.vue -->
<template>
  <link
    href="https://cdn.jsdelivr.net/npm/boxicons@2.0.5/css/boxicons.min.css"
    rel="stylesheet"
  />

  <div class="container">
    <div class="left-panel">
      <h1>Frontend | Creative & Accessible</h1>
      <span class="workshop-auteur"> By Fenna de Wilde </span>
      <p>
        Een oudere studente die als creatieve front-end ontwikkelaar werkt bij
        Bakken en Baeck, een Noors ontwerpbureau voor technologie, deelde enkele
        van haar projecten met me. Ze liet me trots haar eerste project zien en
        besprak ook andere projecten waar ze aan had gewerkt voor BIA (Built in
        Amsterdam). Als student vond ik haar werk buitengewoon interessant, vet
        en creatief.
      </p>

      <p>
        Tijdens haar presentatie toonde ze ook de code voor het implementeren
        van mooie interactieve animaties op webpagina's, waarbij ze speciale
        aandacht besteedde aan toegankelijkheid. Ze benadrukte het belang van
        het toevoegen van ARIA-labels, vooral bij elementen zoals close-icons of
        buttons zonder tekst, en het linken van het logo naar de homepage voor
        duidelijkheid voor screenreaders. Ze deelde inzichten over
        ARIA-controls, ARIA-expanded, ARIA-live en ARIA-atomic. Wat carrousels
        betreft, legde ze uit dat het lastig kan zijn om ze toegankelijk te
        maken, maar gaf tips zoals het gebruik van de role "region" en het
        semantische element "section" voor de carrouselcontainer.
      </p>

      <p>
        Verder benadrukte ze het belang van een rolbeschrijving en het gebruik
        van aria-labelledby of aria-label voor een duidelijke verwijzing naar de
        carrousel. Haar presentatie richtte zich ook op contrast, screenreaders,
        laaggeletterden en hoe je animaties en code kunt implementeren met het
        oog op toegankelijkheid, zodat alle gebruikers de website effectief
        kunnen gebruiken.
      </p>
    </div>

    <div class="right-panel">
      <img src="assets/img/image11.png" alt="Workshop Afbeelding" id="img" />
      <span class="workshop-date">19 jan 2024</span>
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

.workshop-auteur {
  font-size: 15px;
  color: var(--color-1);
}

.workshop-date {
  font-size: larger;
  margin-top: 10px;
  color: var(--color-1);
}

.left-panel {
  display: flex;
  flex-direction: column;
  margin-right: 20px;
  line-height: 1.6;

  border: 1px solid var(--color-1);
  padding: 10px;
  border-radius: 20px;
}

.right-panel {
  display: flex;
  flex-direction: column;
}

img {
  max-width: 100%;
  height: auto;
  border-radius: 20px;
}

p {
  margin-top: 15px;
  font-size: 20px;
  margin-right: 3px;
}

@media only screen and (max-width: 768px) {
  .container {
    grid-template-columns: repeat(1, 2fr);
  }

  .right-panel {
    display: none;
  }
}
</style>
