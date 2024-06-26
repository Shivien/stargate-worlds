## Attributs

```dataviewjs
const attributes = [
	{ name: "Agilité", val: "d4", cost: 0 },
	{ name: "Âme", val: "d4", cost: 0 },
	{ name: "Force", val: "d4", cost: 0 },
	{ name: "Intellect", val: "d4", cost: 0 },
	{ name: "Vigueur", val: "d4", cost: 0 },
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
	{ name: "Athlétisme*", attr: "AGI", val: "d4", cost: 0 },
	{ name: "Combat", attr: "AGI", val: "", cost: 0 },
	{ name: "Culture générale*", attr: "INT", val: "d4", cost: 0 },
	{ name: "Discrétion*", attr: "AGI", val: "d4", cost: 0 },
	{ name: "Éducation", attr: "INT", val: "", cost: 0 },
	{ name: "Intimidation", attr: "AME", val: "", cost: 0 },
	{ name: "Perception*", attr: "INT", val: "d4", cost: 0 },
	{ name: "Performance", attr: "AME", val: "", cost: 0 },
	{ name: "Persuasion*", attr: "AME", val: "d4", cost: 0 },
	{ name: "Pilotage", attr: "AGI", val: "", cost: 0 },
	{ name: "Provocation", attr: "INT", val: "", cost: 0 },
	{ name: "Recherche", attr: "INT", val: "", cost: 0 },
	{ name: "Soins", attr: "INT", val: "", cost: 0 },
	{ name: "Stratégie", attr: "INT", val: "", cost: 0 },
	{ name: "Subterfuge", attr: "AGI", val: "", cost: 0 },
	{ name: "Survie", attr: "INT", val: "", cost: 0 },
	{ name: "Technologie", attr: "INT", val: "", cost: 0 },
	{ name: "Tir", attr: "AGI", val: "", cost: 0 },
];

const skillsCost = skills.reduce((acc, cur) => acc + cur.cost, 0);

dv.table(
	["Nom", "Attribut", "Valeur", `Coût (${skillsCost})`],
	skills.map(s => [s.name, s.attr, s.val, s.cost])
);
```

## Handicaps
## Atouts
## Équipements
