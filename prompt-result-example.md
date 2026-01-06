## Ancien HTML
```html
<div style="max-width: 800px; margin: 0 auto; font-size: 16px; text-align: justify;"><!-- Titre principal -->
<h2 style="text-align: left; font-size: 20px; margin-bottom: 20px;"><b>How does opt-in work?</b></h2>
<!-- Bloc mascotte + bulle -->
<table style="width: 100%; border-collapse: collapse; border: 0; margin-bottom: 30px;">
<tbody>
<tr>
<td style="text-align: center; border: 0;"><img src="/static/S1_L73_Illu_EN-8.png" alt="Opt-in is simple: it works in 3 easy steps, like a winning recipe!" style="max-width: 420px; height: auto;" /></td>
</tr>
</tbody>
</table>
<!-- 3 étapes en colonnes -->
<table style="width: 100%; border-collapse: collapse; border: 0; text-align: center;">
<tbody>
<tr><!-- Étape 1 -->
<td style="width: 33%; vertical-align: top; padding: 10px; border: 0;">
<h3 style="font-size: 18px; margin-top: 0; margin-bottom: 5px;"><b>Step 1</b></h3>
<img src="/static/picto_user.png" alt="Icon step 1" style="width: 60px; height: auto; margin-bottom: 10px;" />
<p style="margin-top: 0; text-align: justify;">After creating an opt-in, the administrator can link one or several processors to it.</p>
</td>
<!-- Étape 2 -->
<td style="width: 33%; vertical-align: top; padding: 10px; border: 0;">
<h3 style="font-size: 18px; margin-top: 0; margin-bottom: 5px;"><b>Step 2</b></h3>
<img src="/static/picto_pc.png" alt="Icon step 2" style="width: 60px; height: auto; margin-bottom: 10px;" />
<p style="margin-top: 0; text-align: justify;">The administrator configures the processor by adding the name, title, subtitle, description, and the data that will be transmitted.</p>
</td>
<!-- Étape 3 -->
<td style="width: 33%; vertical-align: top; padding: 10px; border: 0;">
<h3 style="font-size: 18px; margin-top: 0; margin-bottom: 5px;"><b>Step 3</b></h3>
<img src="/static/picto_pc_pouce.png" alt="Icon step 3" style="width: 60px; height: auto; margin-bottom: 10px;" />
<p style="margin-top: 0; text-align: justify;">This information is then displayed in the widget for transparency purposes.</p>
</td>
</tr>
</tbody>
</table>
</div>
<p><p></p>
```

## Nouveau HTML (avec mini-framework CSS)
```html
<div style="max-width: 800px; margin: 0 auto; font-size: 16px; text-align: justify;">
  <!-- Titre principal -->
  <h2 class="text-left mb-6" style="font-size: 20px;"><b>How does opt-in work?</b></h2>

  <!-- Bloc mascotte + bulle -->
  <div class="text-center mb-6">
    <img src="/static/S1_L73_Illu_EN-8.png" alt="Opt-in is simple: it works in 3 easy steps, like a winning recipe!" style="max-width: 420px; height: auto;" />
  </div>

  <!-- 3 étapes en colonnes -->
  <div class="flex flex-wrap gap-6">
    <!-- Étape 1 -->
    <div class="w-1/3 sm:w-full text-center p-2">
      <h3 style="font-size: 18px; margin-top: 0; margin-bottom: 5px;"><b>Step 1</b></h3>
      <img src="/static/picto_user.png" alt="Icon step 1" style="width: 60px; height: auto; margin-bottom: 10px;" />
      <p class="text-justify" style="margin-top: 0;">After creating an opt-in, the administrator can link one or several processors to it.</p>
    </div>
    <!-- Étape 2 -->
    <div class="w-1/3 sm:w-full text-center p-2">
      <h3 style="font-size: 18px; margin-top: 0; margin-bottom: 5px;"><b>Step 2</b></h3>
      <img src="/static/picto_pc.png" alt="Icon step 2" style="width: 60px; height: auto; margin-bottom: 10px;" />
      <p class="text-justify" style="margin-top: 0;">The administrator configures the processor by adding the name, title, subtitle, description, and the data that will be transmitted.</p>
    </div>
    <!-- Étape 3 -->
    <div class="w-1/3 sm:w-full text-center p-2">
      <h3 style="font-size: 18px; margin-top: 0; margin-bottom: 5px;"><b>Step 3</b></h3>
      <img src="/static/picto_pc_pouce.png" alt="Icon step 3" style="width: 60px; height: auto; margin-bottom: 10px;" />
      <p class="text-justify" style="margin-top: 0;">This information is then displayed in the widget for transparency purposes.</p>
    </div>
  </div>
</div>
```
