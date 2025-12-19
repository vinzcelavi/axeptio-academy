# Ancien HTML

```html
<style>
.two-columns {
  display: flex;
  flex-wrap: wrap;
  width: 100%;
  gap: 1rem;
  margin-top: 25px;
}

.two-columns__left {
  flex: 1 1 300px;
  font-size: 16px;
}

.two-columns__left h3 {
  font-size: 20px;
  margin-top: 0;
  margin-bottom: 10px;
  text-align: left;
}

.two-columns__left p:first-of-type {
  margin-top: 0;
}

.two-columns__right {
  flex: 0 0 120px;
}

.two-columns__right img {
  width: 80px;
  height: auto;
}

@media (max-width: 500px) {
  .two-columns {
    flex-direction: column-reverse;
  }

  .two-columns__right {
    flex: 1 1 100%;
  }
}
</style>

<div style="max-width: 800px; margin: 0 auto; font-size: 16px; text-align: justify;">
  <!-- Bloc 1 : Illustration registre de consentement -->
  <table style="width: 100%; border-collapse: collapse; border: 0; margin-bottom: 20px;">
    <tbody>
      <tr>
        <td style="text-align: center; border: 0;">
          <img src="/static/S1_L17_Illu_FR.png"
               alt="Chez Axeptio, chaque consentement est enregistré dans un registre accessible à tout moment."
               style="max-width: 420px; height: auto;" />
        </td>
      </tr>
    </tbody>
  </table>

  <!-- Bloc 2 : Contenu du registre -->
  <p style="margin-top: 0;">
    <b>Vous pouvez y retrouver les informations suivantes&nbsp;:</b>
  </p>

  <ul style="margin-top: 5px; padding-left: 20px;">
    <li><b>L’horodatage</b> : la date et l’heure précises où le choix a été fait.</li>
    <li><b>Le contexte</b> : sur quelle page et dans quelle situation l’utilisateur a donné (ou refusé) son accord.</li>
    <li><b>L’agent utilisateur</b> : les informations techniques du navigateur et de l’appareil utilisé.</li>
    <li><b>Le statut du consentement</b> : acceptation, refus, modification…</li>
  </ul>

<div class="two-columns">
  <div class="two-columns__left">
    <h3><b>Mais comment retrouver les preuves de consentement&nbsp;?</b></h3>
    <p>
      Les preuves de consentement sont <b>cryptées</b>, <b>stockées dans l'UE</b> et
      <b>conservées</b> conformément à la configuration du client (généralement 13 mois).
    </p>
    <p>
      Vous avez la possibilité <b>d'exporter les journaux au format CSV</b> à des fins d'audit
      ou d'examen interne.
    </p>
    <p style="margin-top: 15px; text-align: left;">
      <i>Besoin d'aide&nbsp;?</i>
      <a href="/static/Procedure-token.pdf" target="_blank">
        Cliquez ici pour télécharger le document qui explique comment accéder à vos consentements.
      </a>
    </p>
  </div>
  <div class="two-columns__right">
    <img src="/static/Cookie-Wonder.png" alt="Mascotte se posant des questions" />
  </div>
</div>
</div>
```

# Nouveau HTML
```html
ici
```
