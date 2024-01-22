<!-- components/Freelance workshop.vue -->
<template>
    <link
      href="https://cdn.jsdelivr.net/npm/boxicons@2.0.5/css/boxicons.min.css"
      rel="stylesheet"
    />
  
    <div class="container">
      <div class="left-panel">
        <h1>FreeLancen</h1>
        <span class="workshop-auteur">By Tim Borst</span>
        <p>
          Tim Borst heeft een inspirerende We Love Web lezing gegeven over
          freelancen, waarbij hij zijn rijke ervaring als front-end ontwerper
          deelde. Tijdens de presentatie nam Tim ons mee door zijn
          carrièreverloop, met bijzondere aandacht voor zijn periode als eigenaar
          van zijn eigen bedrijf. Hij deelde waardevolle inzichten over het leiden
          van een eigen onderneming en benadrukte hoe belangrijk het is om soms
          strenger te zijn tegenover je medewerkers, terwijl je toch een balans
          moet vinden tussen strengheid en empathie. Tim bood een realistische
          kijk op het ondernemerschap in de wereld van front-end design, en zijn
          lezing zal ongetwijfeld velen hebben geïnspireerd die geïnteresseerd
          zijn in freelancen en ondernemerschap.
        </p>
      </div>
  
      <div class="right-panel">
        <img
          src="assets/img/freelance.jpeg"
          alt="Workshop Afbeelding"
          id="img"
        />
        <span class="workshop-date">6 oct 2023</span>
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
  