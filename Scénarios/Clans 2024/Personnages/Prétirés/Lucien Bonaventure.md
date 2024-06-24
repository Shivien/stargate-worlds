## Attributs

```dataviewjs
const attributes = [
	{ name: "Agilité", val: "d6", cost: 1 },
	{ name: "Âme", val: "d6", cost: 1 },
	{ name: "Force", val: "d4", cost: 0 },
	{ name: "Intellect", val: "d10", cost: 3 },
	{ name: "Vigueur", val: "d6", cost: 1 },
];

const attributesCost = attributes.reduce((acc, cur) => acc + cur.cost, 0);

dv.table(
	["Nom", "Valeur", `Coût (${attributesCost})`],
	attributes.map(s => [s.name, s.val, s.cost])
);
```
## Compétences

```dataviewjs
const skills = [
	{ name: "Athlétisme*", attr: "AGI", val: "d6", cost: 1 },
	{ name: "Combat", attr: "AGI", val: "d4", cost: 1 },
	{ name: "Culture générale*", attr: "INT", val: "d8", cost: 2 },
	{ name: "Discrétion*", attr: "AGI", val: "d4", cost: 0 },
	{ name: "Éducation", attr: "INT", val: "d8", cost: 3 },
	{ name: "Intimidation", attr: "AME", val: "", cost: 0 },
	{ name: "Perception*", attr: "INT", val: "d8", cost: 2 },
	{ name: "Performance", attr: "AME", val: "", cost: 0 },
	{ name: "Persuasion*", attr: "AME", val: "d4", cost: 0 },
	{ name: "Pilotage", attr: "AGI", val: "", cost: 0 },
	{ name: "Provocation", attr: "INT", val: "d6", cost: 2 },
	{ name: "Recherche", attr: "INT", val: "d8", cost: 3 },
	{ name: "Soins", attr: "INT", val: "d4", cost: 1 },
	{ name: "Stratégie", attr: "INT", val: "", cost: 0 },
	{ name: "Subterfuge", attr: "AGI", val: "d6", cost: 2 },
	{ name: "Survie", attr: "INT", val: "", cost: 0 },
	{ name: "Technologie", attr: "INT", val: "d10", cost: 4 },
	{ name: "Tir", attr: "AGI", val: "d4", cost: 1 },
];

const skillsCost = skills.reduce((acc, cur) => acc + cur.cost, 0);

dv.table(
	["Nom", "Attribut", "Valeur", `Coût (${skillsCost})`],
	skills.map(s => [s.name, s.attr, s.val, s.cost])
);
```

## Handicaps

- Curieux (majeur)
- Hésitant (mineur)
- Bavard
## Atouts

- Débrouillard
- Provocateur

## Équipements
