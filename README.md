# Axeptio Academy

## Le CSS dans les modules :
```css
/* Layout */
.flex { display: flex; }
.flex-wrap { flex-wrap: wrap; }
.flex-col { flex-direction: column; }
.gap-6 { gap: 1.5rem; }

/* Justify / Align */
.justify-center { justify-content: center; }
.items-center { align-items: center; }

/* Flex width sizing - relative */
.flex-1 { flex: 1 1 0%; }
.w-1\/2 { flex: 0 0 45%; max-width: 45%; }
.w-1\/3 { flex: 0 0 30%; max-width: 30%; }
.w-full { flex: 0 0 100%; max-width: 100%; }

/* Flex width sizing - fixed */
.w-80 { flex: 0 0 80px; max-width: 80px; }
.w-120 { flex: 0 0 120px; max-width: 120px; }
.w-160 { flex: 0 0 160px; max-width: 160px; }
.w-200 { flex: 0 0 200px; max-width: 200px; }
.w-300 { flex: 0 0 300px; max-width: 300px; }

/* Text */
.text-center { text-align: center; }
.text-left { text-align: left; }
.text-justify { text-align: justify; }

/* Spacing */
.mt-auto { margin-top: auto; }
.mt-4 { margin-top: 1rem; }
.mt-6 { margin-top: 1.5rem; }
.mb-4 { margin-bottom: 1rem; }
.mb-6 { margin-bottom: 1.5rem; }
.p-2 { padding: 0.5rem; }
.p-4 { padding: 1rem; }

/* Mobile */
@media (max-width: 500px) {
  .sm\:w-full { 
    flex: 1 1 100%; 
    max-width: 100%; 
  }
  .sm\:flex-col-reverse { 
    flex-direction: column-reverse; 
  }
  .sm\:order-first { 
    order: -1; 
  }
}
```

## Helpers “utility-first” XBlock (façon Tailwind)

Ces utilitaires sont **scopées uniquement par** `.xblock-student_view-html` (voir `src/_xblock-article.scss`).

Vous composez la mise en page en empilant des classes (comme avec Tailwind). Les variantes responsives utilisent le préfixe `sm:` et s'appliquent en dessous de **500px**.

### Layout

- **`flex`**: `display:flex`
- **`flex-wrap`**: `flex-wrap: wrap`
- **`flex-col`**: `flex-direction: column`
- **`gap-6`**: `gap: 1.5rem` (24px)

### Justify / align

- **`justify-center`**: `justify-content: center`
- **`items-center`**: `align-items: center`

### Largeur des colonnes

- **`flex-1`**: `flex: 1 1 0%` (fills remaining space, but wraps nicely)
- **`w-1/2`**: `50%` + `max-width: 45%`
- **`w-1/3`**: `33%` + `max-width: 30%`
- **`w-80` / `w-120` / `w-160` / `w-200` / `w-300`**: fixed width columns (px)
- **`w-full`**: `width: 100%`

### Alignement du text

- **`text-left` / `text-center` / `text-justify`**

### Espacement

- **`mt-auto`**, **`mt-4`**, **`mt-6`**, **`mb-4`**, **`mb-6`**, **`p-2`**, **`p-4`**

### Responsive (< 500px)

- **`sm:w-full`**: force full width (`width: 100%`)
- **`sm:flex-col-reverse`**: reverse stacking order on mobile (`flex-direction: column-reverse`)

### Exemples de layouts

#### 2 colonnes (desktop) → empilées (mobile)

```html
<div class="flex flex-wrap w-full gap-6">
  <div class="w-1/2 sm:w-full">Left column</div>
  <div class="w-1/2 sm:w-full">Right column</div>
</div>
```

Desktop
```
| Left (~45%) | gap | Right (~45%) |
```

Mobile (<500px)
```
| Left  (100%) |
| Right (100%) |
```

#### 2 colonnes + ordre inversé sur mobile

```html
<div class="flex flex-wrap w-full gap-6 sm:flex-col-reverse">
  <!-- Desktop: A then B | Mobile (<500px): B then A -->
  <div class="w-1/2 sm:w-full">Column A</div>
  <div class="w-1/2 sm:w-full">Column B</div>
</div>
```

Desktop
```
| A | gap | B |
```

Mobile (<500px)
```
| B |
| A |
```

#### Colonne de gauche 80px / colonne de droite prend le reste

```html
<div class="flex flex-wrap w-full gap-6">
  <div class="w-80 sm:w-full">[icon]</div>
  <div class="flex-1 sm:w-full">Some longer text content…</div>
</div>
```

Desktop
```
| [80px] | gap | content (flex) |
```

Mobile (<500px)
```
| [icon]   (100%) |
| content  (100%) |
```
