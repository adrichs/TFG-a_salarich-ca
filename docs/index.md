---
layout: splash
title: "Treball Final de Grau - Adrià Salarich"
header: 
  overlay_image: /assets/images/splash.jpg
  overlay_filter: 0.15
  caption: "<i>Bacillus subtilis</i> CotA"
  actions:
    - label: "Llegeix l'<i>Abtsract</i>"
      url: /abstract/
    - label: "Repositori a GitHub"
      url: https://github.com/adrichs/TFG-a_salarich
excerpt: "Millorant el disseny racional de les lacases"
---

# **Un anàlisi *in silico* de determinants de termoestabilitat de les lacases per a la millora del seu disseny racional**

Benvinguts a la pàgina web per a aquest treball final de grau! 

Les **lacases** son enzims àmpliament distribuits a la natura, capaços de degradar un gran ventall de substrats. Gràcies a aquesta propietat, poden ser extremadament útils en ***bioremediació***. 

> ######  ***Què és la bioremediació?***
La bioremediació fa referència al tractament de diferents contaminants mitjançant
l'ús de microorganismes o els enzims que produeixen, capaços de degradar aquests
contaminants en compostos menys nocius.

Malauradament, moltes lacases no són gaire resistents a la calor, cosa que
restringeix la seva aplicació pràctica. Per aquest motiu, aquest projecte
es va proposar trobar allò que diferencia les lacases amb aquesta propietat
a nivell estructural i fisicoquímic.


Per aconseguir-ho, es van seleccionar lacases termostables i no termostables
de diferents bases de dades, es van alinear les seves seqüències i es van comparar mitjançant tests
estadístics i la divergència de Kullback-Leibler.

> ###### ***Què és la divergència de Kullback-Leibler?***
La divergència de Kullback-Leibler és una mesura matemàtica de com de diferents
són dues distribucions de probabilitat entre si. En el context d'aquest
projecte, es va utilitzar per comparar la freqüència de cadascun dels 20
aminoàcids en posicions equivalents entre lacases termostables i no termostables.
Un valor més elevat de la divergència de Kullback-Leibler en una posició determinada
indica que els dos grups de lacases tendeixen a utilitzar aminoàcids diferents
en aquella posició, la qual cosa la converteix en una eina útil per identificar
les posicions que més difereixen entre enzims termostables i no termostables.

A través d'aquests tests, el projecte va descobrir que les lacases termostables i
no termostables són en general molt similars, però
les variacions en l'ús d'aminoàcids específics en posicions concretes
revelen que la termostabilitat pot estar determinada per un petit nombre de
localitzacions clau en l'estructura proteica, més que per diferències
generalitzades en la composició. Moltes d'aquestes posicions es troben en regions
flexibles de la proteïna, com ara els bucles que connecten elements estructurals
més rígids, cosa que suggereix que les lacases termostables poden assolir
la seva estabilitat fixant regions que d'altra manera es mourien massa lliurement
a temperatures elevades.

La identificació d'aquestes posicions és el primer pas cap a l'enginyeria de
lacases més termostables i, per tant, més **útils**
en aplicacions reals de bioremediació.
