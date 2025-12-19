# Ancien HTML

```html
<style>
.two-columns {
  display: flex;
  flex-wrap: wrap;
  width: 100%;
  gap: 1rem;
  margin-top: 10px;
  margin-bottom: 20px;
}

.two-columns__left {
  flex: 0 0 120px;
  text-align: center;
  display: flex;
  align-items: center;
  justify-content: center;
}

.two-columns__left img {
  width: 80px;
  height: auto;
}

.two-columns__right {
  flex: 1 1 300px;
}

.two-columns__right ul {
  margin-top: 0;
  padding-left: 20px;
}

@media (max-width: 500px) {
  .two-columns__left {
    flex: 1 1 100%;
  }
}
</style>
<div style="max-width: 800px; margin: 0 auto; font-size: 16px; text-align: justify;">

  <!-- Titre -->
  <h2 style="text-align: center; font-size: 20px; margin-bottom: 25px;">
    <b>Quelles sont les données collectées&nbsp;?</b>
  </h2>

<div class="two-columns">
  <div class="two-columns__left">
    <img src="/static/picto_loupe.png" alt="Picto données collectées" />
  </div>
  <div class="two-columns__right">
    <ul>
      <li>
        <b>Les pages vues</b> : Chaque fois qu'un utilisateur arrive sur une page de votre site
        et qu'elle se charge, cela constitue une page vue. C'est le point de départ du parcours
        utilisateur et la base pour mesurer vos autres indicateurs de consentement.
      </li>
      <li>
        <b>Le taux d'opt-in</b> : Il s'agit du pourcentage d'utilisateurs qui expriment un
        consentement positif. C'est un indicateur clé de la confiance que vos visiteurs
        accordent à votre marque et à la transparence de votre CMP.
      </li>
      <li>
        <b>Le consentement</b> : L'état de la décision de l'utilisateur — acceptation
        complète, refus ou consentement partiel. Cette granularité permet de respecter les
        choix des utilisateurs tout en collectant uniquement les données autorisées.
      </li>
      <li>
        <b>Le taux d'interaction</b> : Mesure si l'utilisateur interagit ou non avec le widget
        (scroll, clic, navigation). C'est un reflet de l'engagement : plus il est élevé, plus
        vos visiteurs prennent le temps de comprendre et de gérer leurs préférences.
      </li>
      <li>
        <b>Le taux de rebond (dans le cadre du widget)</b> : Indique la proportion
        d'utilisateurs qui quittent le site sans interagir avec la bannière ou le widget de
        consentement. Un taux de rebond élevé peut signaler un besoin d'optimiser
        l'expérience utilisateur (ergonomie, clarté, design).
      </li>
    </ul>
  </div>
</div>

  <!-- Texte complémentaire -->
  <p style="margin-top: 10px;">
    Les appareils (mobile, ordinateur), les campagnes (compatibilité avec le balisage UTM) et les
    configurations (version du widget affichée) sont également pris en compte.
  </p>

  <p style="margin-top: 10px;">
    <b>Ces données alimentent les tableaux de bord internes et les efforts d’optimisation.</b>
  </p>

</div>
```

# Nouveau HTML

```html
ici
```
