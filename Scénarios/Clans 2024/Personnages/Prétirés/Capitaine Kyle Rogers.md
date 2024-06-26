Humain extraterrestre recruté par Apophis pour former une troupe de non Jaffa. Le but était que cette troupe puisse infiltrer la Tau'ri en se faisant passer pour des soldats du SGC.
SG1 a découvert le camp d'entrainement. Celui-ci avait été abandonné par les maîtres Jaffas parti pour combattre au côté d'Apophis. SG1 a réussi a les convaincre d'abandonner leur entrainement.
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
	{ name: "Discrétion*", attr: "AGI", val: "d8", cost: 2 },
	{ name: "Éducation", attr: "INT", val: "", cost: 0 },
	{ name: "Intimidation", attr: "AME", val: "d6", cost: 3 },
	{ name: "Perception*", attr: "INT", val: "d6", cost: 1 },
	{ name: "Performance", attr: "AME", val: "", cost: 0 },
	{ name: "Persuasion*", attr: "AME", val: "d6", cost: 1 },
	{ name: "Pilotage", attr: "AGI", val: "d4", cost: 1 },
	{ name: "Provocation", attr: "INT", val: "", cost: 0 },
	{ name: "Recherche", attr: "INT", val: "", cost: 0 },
	{ name: "Soins", attr: "INT", val: "d6", cost: 2 },
	{ name: "Stratégie", attr: "INT", val: "d6", cost: 2 },
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

- **Impulsif (Majeur) :** fonce sans réfléchir.
- **Loyal (Mineur) :** loyal envers ses amis et ses alliés.
## Atouts

- **Esquive :** -2 aux attaques à distance contre le personnage.
- **Rock'n roll ! :** ignore la pénalité de recul en cas de tir avec une cadence supérieure ou égale à 2.
- **Véloce :** +2 en Allure et le dé de course est un d8.

## Équipements

- Veste en kevlar (torse) : +2 en Armure.
- Grenade : portée 4/8/16, dégât 3d6, gabarit moyen.
- MP5 : 12/24/48, 2d6 PA 1, CDT 3, 30 coups, Force min. d6.
- Glock : 12/24/48, 2d6 PA 1, 17 coups.