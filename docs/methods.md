---
layout: single
title: "Mètodes"
permalink: /methods/
---

Les lacases termostables i no termostables es van recopilar de UniProt,
NCBI i BRENDA utilitzant els filtres que proporcionen aquestes bases de dades.
Les seqüències proteiques es van descarregar en format FASTA mitjançant un script
de bash.

Per reduir la redundància de seqüències dins dels grups, les seqüències es van
agrupar amb CD-HIT en grups representatius més petits.

A continuació, es van construir alineaments múltiples de seqüències de lacases
termostables i no termostables utilitzant MAFFT. Per millorar-ne la qualitat
i la usabilitat posterior, els alineaments es van retallar amb trimAl.

L'accessibilitat al solvent de cada residu en l'estructura de la CotA de
*B. subtilis* (PDB: 1GSK) es va calcular amb FreeSASA. Els residus es van
classificar com a enterrats o accessibles al solvent en funció d'un llindar
d'accessibilitat relativa al solvent del 20% i es van exportar des de ChimeraX.

> ##### ***Què és l'accessibilitat al solvent?***
> L'accessibilitat al solvent mesura el grau d'exposició d'un aminoàcid determinat
> a les molècules d'aigua del seu entorn. S'expressa com a percentatge de l'exposició
> màxima possible per a aquell aminoàcid. Un valor proper al 0% significa que el
> residu es troba profundament enterrat dins la proteïna, mentre que un valor proper
> al 100% indica que està completament exposat a la superfície. Aquesta distinció és
> important perquè els residus enterrats i els de superfície tenen papers molt
> diferents en l'estructura i l'estabilitat de la proteïna.

Les matrius de puntuació específiques de posició (PSSM) es van generar a partir dels
alineaments retallats utilitzant goalign. Prenent CotA com a referència, les files
de la PSSM corresponents als residus enterrats i accessibles al solvent es van
extreure per separat per a ambdós conjunts de dades mitjançant un script de Python
personalitzat.

Es van aplicar tres anàlisis complementàries per comparar els dos grups.
L'enriquiment de grups d'aminoàcids es va avaluar mitjançant tests de Chi-quadrat,
les propietats fisicoquímiques es van comparar amb el test t de Student i el test
de Mann-Whitney U, i la divergència de Kullback-Leibler es va utilitzar per
identificar les posicions que més difereixen entre lacases termostables i no
termostables.

Les posicions més discriminants es van cartografiar sobre l'estructura 1GSK
mitjançant ChimeraX i el seu context estructural es va examinar per interpretar
el seu possible paper en la termostabilitat.
