---
title: Transformace
demand: 2
hasSolution: false
---

Použijte opět pole `numbers`, `names` a `persons` z předchozího cvičení.

1. Pomocí metody `filter` získejte z pole `numbers` pouze ta čísla, která jsou sudá a uložte je do proměnné `evenNumbers`. Vypište toto nové pole do konzole.
1. Pomocí metody `filter` získejte z pole `persons` pouze dospělé lidi a uložte je do proměnné `adults`. Vypište toto nové pole do konzole.
1. Pomocí metody `map` vydělte všecha čísla v poli `numbers` třemi a uložte je do proměnné `dividedByThree`. Vypište toto nové pole do konzole.
1. Pomocí metody `map` převeďte všechna čísla z pole `numbers` na řetězec. Výsledek vypište do konzole.
1. Z pole `persons` pomocí metody `map` vytvořte pro každou osobu email ve formátu `petr@gmail.com`, a výsledek uložte do proměnné `emails`. Vypište toto nové pole do konzole.
1. Z pole `persons` pomocí metody `map` vytvořte pro každou osobu položku HTML seznamu ve formátu `<li>Petr (16)</li>`, a výsledek uložte do proměnné `list`. Vypište toto nové pole do konzole.

---solution

```js
// Vytvořte proměnnou evenNumbers. Pomocí metody filter získejte z pole numbers pouze ta čísla, která jsou sudá a uložte je do proměnné evenNumbers. Vypište toto nové pole do konzole.
const evenNumbers = numbers.filter((item) => item % 2 === 0);
console.log(evenNumbers);
​
// Vytvořte proměnnou adults. Pomocí metody filter získejte z pole persons pouze dospělé lidi a uložte je do proměnné adults. Vypište toto nové pole do konzole.
const adults = persons.filter((item) => item.age > 18 );
console.log(adults);
​
// Vytvořte proměnnou dividedByThree. Pomocí metody map vydělte všecha čísla v poli numbers třemi a uložte je do proměnné dividedByThree. Vypište toto nové pole do konzole.
const dividedByThree = numbers.map((item) => item / 3);
console.log(dividedByThree);
​
// Vytvořte proměnnou emails. Z pole persons pomocí metody map vytvořte pro každou osobu email ve formátu petr@gmail.com, a výsledek uložte do proměnné emails. Vypište toto nové pole do konzole.
const emails = persons.map((item) => `${item.name.toLowerCase()}@gmail.com`);
console.log(emails);
```
