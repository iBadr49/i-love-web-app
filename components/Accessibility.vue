<!-- components/Accessibility workshop.vue -->
<template>
  <link
    href="https://cdn.jsdelivr.net/npm/boxicons@2.0.5/css/boxicons.min.css"
    rel="stylesheet"
  />

  <div class="container">
    <div class="left-panel">
      <h1>Accessibility</h1>
      <span class="workshop-auteur">By Ischa Gast</span>
      <p>
        Tijdens deze 'We Love Web'-sessie deelde Ischa Gast waardevolle
        inzichten over webtoegankelijkheid. Hij benadrukte het belang van
        moderne tools om websites toegankelijker te maken. Ischa gebruikte
        interessante voorbeelden uit zijn werk bij Schiphol, waar hij zich richt
        op het verbeteren van de toegankelijkheid van hun website. Zijn
        presentatie werpte een helder licht op de uitdagingen waarmee veel
        websites nog steeds te maken hebben op het gebied van toegankelijkheid.
        Hij inspireerde ons om ons in te zetten voor een inclusievere online
        wereld.
      </p>
    </div>

    <div class="right-panel">
      <img src="assets/img/accessibility.png" alt="Workshop Afbeelding" id="img" />
      <span class="workshop-date">20 oct 2023</span>
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
