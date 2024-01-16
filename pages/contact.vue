<template>
  <link
    href="https://cdn.jsdelivr.net/npm/boxicons@2.0.5/css/boxicons.min.css"
    rel="stylesheet"
  />
  <AppHeader />
  <Backtohome />

  <div class="container">
    <div class="left-panel">
      <h1>Contact us</h1>
      <p>
        Voor informatie over We love web of andere vragen kun je contact
        opnemen:
      </p>
      <p>Telefoonnummer Onderwijsbureau: 020 595 1855</p>
      <p>E-mail: info-fdnd@hva.nl</p>

      <div class="socials">
        <a href="#" target="_blank" rel="noopener noreferrer">
          <i class="bx bxl-twitter"></i>
        </a>
        <a href="#" target="_blank" rel="noopener noreferrer">
          <i class="bx bxl-github"></i>
        </a>
        <a href="#" target="_blank" rel="noopener noreferrer">
          <i class="bx bxl-linkedin"></i>
        </a>
        <a href="#" target="_blank" rel="noopener noreferrer">
          <i class="bx bxl-instagram"></i>
        </a>
      </div>
    </div>
    <div class="right-panel">
      <form>
        <label for="name">Naam:</label>
        <input type="text" id="name" name="name" required />

        <label for="email">Email:</label>
        <input type="email" id="email" name="email" required />

        <label for="message">Bericht:</label>
        <textarea id="message" name="message" required></textarea>

        <button type="submit">Verstuur</button>
      </form>
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

.left-panel {
  display: flex;
  flex-direction: column;
  border-right: 2px solid var(--color-1);
}

.right-panel {
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 10px;
}

form {
  display: flex;
  flex-direction: column;
  width: 40vw;
}

label {
  margin-bottom: 5px;
}

input,
textarea {
  border-radius: 10px;
  border: 1px solid var(--color-1);
  margin-bottom: 15px;
  padding: 8px;
}

label[for="message"] {
  display: block;
  margin-bottom: 5px;
}

#message {
  height: 150px;
  resize: vertical;
}

button {
  width: 20vw;
  background-color: var(--color-2);
  border-radius: 10px;
  border: 1px solid var(--color-1);
  padding: 10px;
  cursor: pointer;
  transition: background-color 0.5s;
}
button:hover {
  background-color: var(--color-1);
  color: white;
}

h1,
p {
  margin-bottom: 10px;
  line-height: 1.6;
}

p {
  font-size: 20px;
  margin-right: 3px;
}

.socials a {
  text-decoration: none;
  color: black;
}

.socials {
  margin-top: 20px;
}

.socials a {
  margin-right: 15px;
  font-size: 1.5em;
  color: black;
}

.socials i:hover {
  color: var(--color-1);
}

@media only screen and (max-width: 768px) {
  .container {
    grid-template-columns: repeat(1, 1fr);
    gap: 30px;
  }

  .right-panel {
    border: 1px solid var(--color-1);
    padding: 20px;

  }

  .left-panel {
    border-right: none;
  }

  form {
    width: 70vw;
  }  
}
</style>
