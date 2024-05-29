Rebelle Jaffa.
## Attributs

```dataviewjs
const attributes = [
	{ name: "Agilité", val: "d8", cost: 2 },
	{ name: "Âme", val: "d6", cost: 1 },
	{ name: "Force", val: "d8", cost: 2 },
	{ name: "Intellect", val: "d4", cost: 0 },
	{ name: "Vigueur", val: "d8", cost: 2 },
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
	{ name: "Combat", attr: "AGI", val: "d10", cost: 5 },
	{ name: "Culture générale*", attr: "INT", val: "d4", cost: 0 },
	{ name: "Discrétion*", attr: "AGI", val: "d4", cost: 0 },
	{ name: "Éducation", attr: "INT", val: "", cost: 0 },
	{ name: "Intimidation", attr: "AME", val: "d6", cost: 2 },
	{ name: "Perception*", attr: "INT", val: "d4", cost: 0 },
	{ name: "Performance", attr: "AME", val: "", cost: 0 },
	{ name: "Persuasion*", attr: "AME", val: "d4", cost: 0 },
	{ name: "Pilotage", attr: "AGI", val: "d8", cost: 3 },
	{ name: "Provocation", attr: "INT", val: "", cost: 0 },
	{ name: "Recherche", attr: "INT", val: "", cost: 0 },
	{ name: "Soins", attr: "INT", val: "", cost: 0 },
	{ name: "Stratégie", attr: "INT", val: "d4", cost: 1 },
	{ name: "Survie", attr: "INT", val: "d6", cost: 3 },
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

- **Code d’Honneur (Majeur) :** tient parole et agit comme un gentleman.
## Atouts

- **Immunité aux maladies**
- **Régénération** : un jet de guérison naturelle par jour (au lieu d'une fois tous les 5 jours).
- **Dépendance** : larve [[Goa'uld]].
## Équipements
