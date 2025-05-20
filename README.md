# 51 pontos visszaesési jel - HTML kérdőív

Ez az oldal egy 51 kérdésből álló, IGEN/NEM alapú visszaesési kockázatot vizsgáló kérdőív. A válaszok alapján az oldal pontszámot számít, megjeleníti diagramon a korábbi eredményeket, és biztonsági mentést is végez automatikusan.

---

## Fő funkciók:

### ✅ Kérdőív
- 51 kérdés, mindegyik IGEN/NEM választhatósággal.
- Minden IGEN válasz a sorszámával egyező pontszámot ér.
- A maximális pontszám: **1356**.

### ✅ Pontszámítás
- A "**Eredmény megjelenítése**" gomb
  - üsszeszámolja a pontokat
  - megjeleníti a pontszámot szövegesen
  - frissíti a diagramot
  - **automatikusan letölti** a biztonsági mentést `.json` formátumban (`kitoltesek.json`)

---

## Gombok funkciója:

### 🔢 **Eredmény megjelenítése**
- A kérdőív pontszámának kiszámítása
- A pontszám és a visszaesési trend megjelenítése diagramon
- Mentés automatikusan: `kitoltesek.json`

### 📂 **Korábbi eredmények betöltése**
- Egy `.json` állomány kiválasztása
- A diagram frissítése a betöltött adatokkal

### ❌ **Összes eredmény törlése**
- Törli a localStorage-ban tárolt összes kitöltést
- Eltávolítja a diagramot
- Az éppen megadott pontszámot is eltávolítja

---

## Diagram
- Minden beküldés után frissül
- Az X tengely a **kitöltés dátuma**
- Az Y tengely a **pontszám** (0–1356)

---

## Mentés
- A rendszer minden kitöltés után automatikusan menti az adatokat a böngésző alapértelmezett letöltések mappába `kitoltesek.json` néven
- A fájl kézzel átnevezhető vagy archiválható

---

## Biztonság
- A rendszer a kitöltés eredményeit a futtatott eszközön tárolja

---

## Mobilhasználat
- A HTML-fájl működik mobilon is, ha **helyileg megnyitod a böngészőben**
- **Google Drive-ból közvetlenül megnyitva nem fut le a kód**

---

## Online használat lehetősége
- Az oldal feltölthető pl. GitHub Pages-re, ahonnan egy linkkel bárki eléri:
  - https://felhasznalonev.github.io/visszaesesi-jel/
- Teljes funkcionalitás működik (pontozás, mentés, visszatöltés, diagram)

---

## Tipp a felhasználónak:
> A letöltött `kitoltesek.json` fájlt javasolt **ugyanabba a mappába helyezni, mint a HTML-fájlt**, hogy később könnyen visszatölthető legyen.
