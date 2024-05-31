Ancien hôte du [[Goa'uld]] Orti qui était un Ashrak (assassin).
## Attributs

```dataviewjs
const attributes = [
	{ name: "Agilité", val: "d8", cost: 2 },
	{ name: "Âme", val: "d8", cost: 2 },
	{ name: "Force", val: "d4", cost: 0 },
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
	{ name: "Athlétisme*", attr: "AGI", val: "d6", cost: 1 },
	{ name: "Combat", attr: "AGI", val: "d8", cost: 3 },
	{ name: "Culture générale*", attr: "INT", val: "d4", cost: 0 },
	{ name: "Discrétion*", attr: "AGI", val: "d8", cost: 2 },
	{ name: "Éducation", attr: "INT", val: "", cost: 0 },
	{ name: "Intimidation", attr: "AME", val: "", cost: 0 },
	{ name: "Perception*", attr: "INT", val: "d4", cost: 0 },
	{ name: "Performance", attr: "AME", val: "", cost: 0 },
	{ name: "Persuasion*", attr: "AME", val: "d8", cost: 2 },
	{ name: "Pilotage", attr: "AGI", val: "d4", cost: 1 },
	{ name: "Provocation", attr: "INT", val: "", cost: 0 },
	{ name: "Recherche", attr: "INT", val: "", cost: 0 },
	{ name: "Soins", attr: "INT", val: "", cost: 0 },
	{ name: "Stratégie", attr: "INT", val: "", cost: 0 },
	{ name: "Subterfuge", attr: "AGI", val: "", cost: 0 },
	{ name: "Survie", attr: "INT", val: "", cost: 0 },
	{ name: "Technologie", attr: "INT", val: "d6", cost: 2 },
	{ name: "Tir", attr: "AGI", val: "d4", cost: 1 },
	{ name: "Artefact Goa'uld", attr: "AME", val: "d6", cost: 2 },
];

const skillsCost = skills.reduce((acc, cur) => acc + cur.cost, 0);

dv.table(
	["Nom", "Attribut", "Valeur", `Coût (${skillsCost})`],
	skills.map(s => [s.name, s.attr, s.val, s.cost])
);
```

## Handicaps

- Cauchemars

## Atouts

- Assassin : +2 aux dégâts si la cible est Vulnérable ou s'il fait une Attaque surprise.
- Hôte Goa'uld : utilisation des artefacts Goa'uld.
## Équipements

- Kara kesh (gant Goa'uld)
	- Rafale
	- Ravage
- Bracelet de guérison
	- Guérison