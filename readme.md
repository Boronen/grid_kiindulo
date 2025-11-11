#basic jegyzet az óráról

##max-width:
1000px; → a konténer nem lehet szélesebb, mint 1000px
##width:
100%; → a konténer kitölti a rendelkezésre álló szélességet

##display:
grid; → rácsos elrendezést használ
##grid-template-columns:
1fr 4fr 1fr; → 3 oszlop, arányok: 1:4:1
##grid-template-rows:
250px 100px auto; → 3 sor, magasság fix- fix- automatikus
##grid-template-areas:
 "h h h" "as ar n" "f f f"; → névvel ellátott rácsterületek, könnyű elhelyezés
##grid-area: 
h; → elem a "h" nevű rácsterületen jelenik meg
gap: 20px; → rács elemei közötti térköz

repeat(auto-fit, minmax(200px, 250px)) → annyi oszlop, amennyi elfér, minimum 200px, maximum 250px
justify-content: space-around; → a rács elemei vízszintesen elosztva, körülöttük térköz

order: -1; → rácsban vagy flexboxban a sorrendet módosítja, negatív = előrébb

transition: background-color 0.3s ease; → színváltozás animálása 0.3 másodperc alatt
text-decoration: none; → link aláhúzás eltávolítása
color: white; / color: rgb(252,144,4); → szöveg színe
padding: 10px 15px; → belső tér a blokk körül
display: block; → elem blokk szintű, az egész sort kitölti

@media screen and (max-width:700px) → ha a képernyő ≤ 700px, akkor ez az elrendezés érvényes

grid-template-columns: 1fr; → egy oszlopos elrendezés

grid-template-areas: → területek egymás alatt