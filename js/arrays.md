# JavaScript Arrays

Your item inventory system - storing and managing collections of data.

## Creating Arrays

```javascript
const champions = ['Graves', 'Kindred', 'Kha\'Zix'];
const teamComp = new Array(5).fill('Available');

console.log(champions);
console.log(teamComp);
```

## Basic Properties & Methods

```javascript
const items = ['Kraken Slayer', 'IE', 'LDR'];

console.log(items.length);
console.log(items.includes('IE'));
console.log(items.includes('Thornmail'));
```

## Adding/Removing Elements

```javascript
const buildOrder = ['Doran\'s Blade'];

buildOrder.push('Kraken Slayer');
buildOrder.push('Berserker\'s Greaves');

console.log(buildOrder);
```

## Splice - The Swiss Army Knife

```javascript
const inventory = ['Health Potion', 'Control Ward', 'Long Sword', 'Pickaxe'];

inventory.splice(2, 1, 'BF Sword');
console.log(inventory);

inventory.splice(1, 0, 'Pink Ward');
console.log(inventory);
```

## Iteration Methods

```javascript
const scores = [15, 3, 8, 12, 1];

// forEach - do something with each element
scores.forEach((kills, playerIndex) => {
    console.log(`Player ${playerIndex + 1}: ${kills} kills`);
});

// map - transform each element, return new array
const kdRatios = scores.map((kills, index) => {
    const deaths = index + 1;
    return (kills / deaths).toFixed(2);
});
console.log(kdRatios);

// filter - keep elements that pass condition
const carries = scores.filter((kills) => {
    return kills >= 10;
});
console.log(carries); // [15, 12]

// reduce - combine all elements into single value
const totalKills = scores.reduce((teamKills, playerKills) => {
    return teamKills + playerKills;
}, 0); // 0 is starting value
console.log(totalKills);
```

## Performance Notes

- **push()** and **pop()** are fast (O(1))
- **unshift()** and **shift()** are slow (O(n)) - avoid when possible
- **splice()** can be slow for large arrays depending on position
- Iteration methods create new arrays (except forEach) - memory friendly for small datasets