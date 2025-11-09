# puzzlefruit

 

<p align="center">
  <img src="https://img.shields.io/badge/JavaScript-Vanilla-yellow" alt="Vanilla JS">
  <img src="https://img.shields.io/badge/Vue.js-3-green" alt="Vue 3">
  <img src="https://img.shields.io/badge/Live-Demo-brightgreen" alt="Live">
  <img src="https://img.shields.io/badge/Algorithms-Conway-blue" alt="Conway">
</p>

**Live demo**: http://maniontg.webd.pro/puzzlefruit/
 
**Pure JS | Canvas**

## Tech stack
- Vanilla JavaScript
- HTML5 Canvas
- CSS Grid/Flexbox
- Vue.js

## Jak uruchomić lokalnie
1. `git clone https://github.com/Komodo2041/puzzlefruit.git`
2. Otwórz `index.html` w przeglądarce
 
Short Video: https://youtube.com/shorts/WHazbhLF880

Ten rodzaj puzzli uznałem za interesujący nie nadaje się on na mobilki

## Dodawanie punktów na postawie ilości pasujących owoców
```js 
function addPoints(pos, table) {
    let res = 0;
    for (let i = 0; i < 6; i++) {
        for (let j = 0; j < 6; j++) {
            if (table[pos[0] + i][pos[1] + j]) {
                res++;
            }
        }
    }
    return res;
}
```