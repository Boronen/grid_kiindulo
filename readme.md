# CSS Grid és Alapvető Stílusok Jegyzet

---

## Konténer méretezés

```css
max-width: 1000px; /* A konténer nem lehet szélesebb, mint 1000px */
width: 100%;       /* A konténer kitölti a rendelkezésre álló szélességet */
```

---

## Grid elrendezés

```css
display: grid; /* Rácsos elrendezés */

grid-template-columns: 1fr 4fr 1fr; /* 3 oszlop, arányok: 1:4:1 */
grid-template-rows: 250px 100px auto; /* 3 sor, magasság: fix-fix-automatikus */
grid-template-areas: 
  "h h h"
  "as ar n"
  "f f f"; /* Névvel ellátott rácsterületek */
grid-area: h; /* Elem a "h" nevű rácsterületen jelenik meg */
gap: 20px; /* Rács elemei közötti térköz */
```

---

## Rugalmas oszlopok

```css
grid-template-columns: repeat(auto-fit, minmax(200px, 250px));
justify-content: space-around; /* A rács elemei vízszintesen elosztva, körülöttük térköz */
```

---

## Sorrend módosítása

```css
order: -1; /* Rácsban vagy flexboxban a sorrendet módosítja, negatív = előrébb */
```

---

## Animáció és szövegstílus

```css
transition: background-color 0.3s ease; /* Színváltozás animálása 0.3s alatt */
text-decoration: none; /* Link aláhúzás eltávolítása */
color: white;          /* Szöveg színe */
color: rgb(252,144,4); /* Szín RGB-ben */
padding: 10px 15px;    /* Belső tér a blokk körül */
display: block;        /* Elem blokk szintű, az egész sort kitölti */
```

---

## Reszponzív design

```css
@media screen and (max-width:700px) {
  grid-template-columns: 1fr; /* Egy oszlopos elrendezés */
  grid-template-areas: 
    "h"
    "as"
    "ar"
    "n"
    "f"; /* Területek egymás alatt */
}
```

---
