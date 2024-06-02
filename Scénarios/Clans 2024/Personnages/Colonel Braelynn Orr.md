## Attributs (5)

```dataviewjs
const attributes = [
	{ name: "Agilité", val: "d8", cost: 2 },
	{ name: "Âme", val: "d6", cost: 1 },
	{ name: "Force", val: "d6", cost: 1 },
	{ name: "Intellect", val: "d6", cost: 1 },
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
	{ name: "Athlétisme*", attr: "AGI", val: "d8", cost: 2 },
	{ name: "Combat", attr: "AGI", val: "d6", cost: 2 },
	{ name: "Culture générale*", attr: "INT", val: "d4", cost: 0 },
	{ name: "Discrétion*", attr: "AGI", val: "d6", cost: 1 },
	{ name: "Éducation", attr: "INT", val: "", cost: 0 },
	{ name: "Intimidation", attr: "AME", val: "d6", cost: 3 },
	{ name: "Perception*", attr: "INT", val: "d6", cost: 1 },
	{ name: "Performance", attr: "AME", val: "", cost: 0 },
	{ name: "Persuasion*", attr: "AME", val: "d6", cost: 1 },
	{ name: "Pilotage", attr: "AGI", val: "d4", cost: 1 },
	{ name: "Provocation", attr: "INT", val: "", cost: 0 },
	{ name: "Recherche", attr: "INT", val: "", cost: 0 },
	{ name: "Soins", attr: "INT", val: "d4", cost: 1 },
	{ name: "Stratégie", attr: "INT", val: "d8", cost: 4 },
	{ name: "Subterfuge", attr: "AGI", val: "", cost: 0 },
	{ name: "Survie", attr: "INT", val: "d6", cost: 2 },
	{ name: "Technologie", attr: "INT", val: "", cost: 0 },
	{ name: "Tir", attr: "AGI", val: "d8", cost: 3 },
];

const skillsCost = skills.reduce((acc, cur) => acc + cur.cost, 0);

dv.table(
	["Nom", "Attribut", "Valeur", `Coût (${skillsCost})`],
	skills.map(s => [s.name, s.attr, s.val, s.cost])
);
```

## Handicaps

- **Code d'honneur (Majeur) :** fonce sans réfléchir.
- **Loyal (Mineur) :** loyal envers ses amis et ses alliés.
## Atouts

- Commandement
- Inspiration
- Leader naturel

## Équipements

- Veste en kevlar (torse) : +2 en Armure.
- Grenade : portée 4/8/16, dégât 3d6, gabarit moyen.
- MP5 : 12/24/48, 2d6 PA 1, CDT 3, 30 coups, Force min. d6.
- Glock : 12/24/48, 2d6 PA 1, 17 coups.