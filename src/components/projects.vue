<template>
  <section id="projets" class="section-body">
    <div class="projets-carte-visite">
      <div class="carte">
        <div class="carte-header">
          <h2>Burgbad Projet</h2>
          <div class="projet_languages">
            <span>VBA</span>
            <span>SQLServer</span>
          </div>
        </div>
        <div class="carte-body">
          <span>Stage</span>
          <p>Logiciel pour gérer les clients et créer des devis, avec une gestion CRUD et base de données SQLServer.</p>
        </div>
      </div>
      <div class="carte">
        <div class="carte-header">
          <h2>OneManga</h2>
          <div class="projet_languages">
            <span>HTML/CSS</span>
            <span>JavaScript</span>
            <span>PHP</span>
          </div>
        </div>
        <div class="carte-body">
          <span>Cours</span>
          <p>Site vitrine pour l'achat de mangas selon les catégories, développé en équipe.</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Projects",
};
</script>

<style scoped>
.projets-carte-visite {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 20px;
  padding: 40px;
  justify-items: center;
}

.carte {
  background-color: #333;
  border-radius: 12px;
  padding: 20px;
  box-shadow: 0 8px 16px rgba(0, 0, 0, 0.3);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  width: 100%;
  max-width: 350px;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.carte:hover {
  transform: scale(1.05);
  box-shadow: 0 12px 24px rgba(0, 0, 0, 0.5);
}

.carte-header h2 {
  color: #cccccc;
  font-size: 22px;
  margin-bottom: 10px;
}

.projet_languages {
  display: flex;
  flex-wrap: wrap;
}

.projet_languages span {
  background-color: #444;
  padding: 5px 10px;
  border-radius: 5px;
  margin-right: 8px;
  margin-bottom: 5px;
  color: #cccccc;
  font-size: 14px;
}

.carte-body p {
  color: #cccccc;

  font-size: 14px;
  line-height: 1.5;
  margin-top: 10px;
}

@media (max-width: 768px) {
  .projets-carte-visite {
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  }
}

</style>
