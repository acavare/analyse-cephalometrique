# Analyse céphalométrique : Tweed, Steiner, Ricketts

Application d'apprentissage de l'analyse céphalométrique sur téléradiographie de profil, destinée aux étudiants en odontologie. Elle réunit les trois analyses que tout étudiant doit connaitre (#OIC 2-19-15 et 2-19-16) : Tweed, Steiner et Ricketts (11 facteurs).

L'application est le fichier, nommé `index.html`, et fonctionne entièrement dans le navigateur, sans installation, sans compte et sans connexion. Aucune image ni aucune donnée ne quitte l'ordinateur car tout est calculé localement.

## Ouvrir l'application

Deux possibilités :

- En ligne, à l'adresse de la page GitHub Pages du dépôt (lien à compléter après publication).
- Hors ligne, en téléchargeant le fichier `index.html`, puis en l'ouvrant d'un double-clic ou par clic droit, « Ouvrir avec » : Google Chrome, Safari, Firefox ou Edge.

La téléradiographie se charge avec le bouton « Ouvrir une image… » ou en la glissant dans la zone centrale (JPG ou PNG). La molette, les boutons +/- ou le pad zoome sur l'image, la barre espace maintenue avec un glisser déplace le cliché, et le bouton « Ajuster » le recentre.

## Déroulé en quatre étapes

Les quatre étapes s'affichent en haut du panneau de droite. Une étape terminée passe au vert.

### 1. Mise à l'échelle

Les mesures angulaires ne demandent aucune échelle mais les mesures linéaires nécessitent cette mise à l'échelle. Repérer sur le cliché un segment de longueur connue, en général la règle radiographique graduée, cliquer « Tracer le segment de référence », placer ses deux extrémités puis saisir sa longueur réelle en millimètres. « Appliquer l'échelle » active les mesures linéaires et ouvre l'étape suivante. 
Attention il est nécessaire de respecter ces deux dernières étapes pour que la mise à l'échelle fonctionne

### 2. Choix de l'analyse

Cocher Tweed, Steiner, Ricketts (11 facteurs), ou plusieurs d'entre elles. Les points céphalométriques communs ne se placent qu'une fois. Pour Ricketts, saisir l'âge du patient : plusieurs normes varient avec l'âge, et sans âge saisi ce sont les normes à 9 ans qui s'appliquent. Le bouton « Commencer les tracés » lance le placement du premier point.

### 3. Placement des points

La liste ne présente que les points utiles aux analyses cochées, avec pour chacun sa définition et les analyses qui l'utilisent. Le compteur indique le nombre de points déjà placés.

Le point demandé s'affiche dans un bandeau en haut du cliché. Un clic sur l'image le place et l'application passe au point suivant. Pour reprendre un point, cliquer dessus dans la liste puis sur sa nouvelle position, ou le faire glisser directement sur le cliché. Après avoir modifié un point, recliquer sur le point suivant de la liste.

Une loupe de précision s'ouvre pendant le placement, le déplacement d'un point et le tracé de l'échelle. Elle montre la zone agrandie autour du curseur avec une croix de visée, ce qui évite de zoomer pour chaque point. Le bouton « Loupe » la désactive.

Les tracés automatiques s'affichent en blanc. Seuls les repères qui guident le placement restent en trait épais : le plan mandibulaire, les axes des incisives et le plan d'occlusion.

### 4. Résultats

Pour chaque analyse cochée, un tableau présente la mesure, la norme, la valeur du patient et son interprétation clinique. Les mesures encore incalculables indiquent les points manquants.

L'analyse de Tweed est complétée par le tableau de difficulté cranio-faciale de Merrifield. L'analyse de Ricketts est complétée par l'indice VERT et la typologie faciale.

Le tableau s'exporte en CSV, se copie pour être collé dans un tableur ou un traitement de texte, et l'image annotée du tracé s'exporte en pleine résolution.

## Les points

Quelques points demandent une attention particulière.

- **Go′ et Br sont des points fictifs.** Go′ sert uniquement à tracer la tangente au bord inférieur de la mandibule passant par Me (plan mandibulaire). Br sert uniquement à tracer la tangente au bord postérieur de la branche passant par Ar, le long de laquelle se mesure la hauteur faciale postérieure de Tweed.
- **Certains points se placent sur une ligne.** Dc se place sur la ligne Ba-Na. R2 se place sur la parallèle à Francfort passant par R1, et R4 sur la parallèle à PtV passant par R3. Une ligne guide en pointillés s'affiche pendant leur placement.
- **Certains points sont construits par l'application** et s'affichent en carrés blancs : Xi, centre du rectangle tracé sur R1 à R4 avec des côtés parallèles à Francfort et à PtV, E et L, projections d'Ar et de Pog sur SN, Ao et Bo, projections de A et B sur le plan d'occlusion fonctionnel.

**Base du crâne**

| Point | Nom | Définition | Analyses |
|---|---|---|---|
| S | Sella | Centre géométrique de la selle turcique | Tweed, Steiner |
| Na | Nasion | Point le plus antérieur de la suture fronto-nasale | Tweed, Steiner, Ricketts |
| Ba | Basion | Point le plus bas et le plus reculé du basi-occipital | Ricketts |
| Po | Porion | Point le plus élevé du conduit auditif externe | Tweed, Ricketts |
| Or | Orbitale | Point le plus déclive du rebord orbitaire | Tweed, Ricketts |
| Pt | Point ptérygoïdien | Bord postéro-supérieur de la fente ptérygo-maxillaire (PtV passe par ce point) | Ricketts |
| Ar | Articulare | Intersection du bord postérieur du ramus et de la face exocrânienne du clivus (sa projection sur SN donne le point E de Steiner) | Tweed, Steiner |
| Co | Condylion | Point le plus postérieur et supérieur du condyle (angle de Mc Horris) | Ricketts |
| Dc | Point Dc | Centre du col du condyle sur la ligne Ba-Na (le point se place sur la ligne) | Ricketts |

**Maxillaire**

| Point | Nom | Définition | Analyses |
|---|---|---|---|
| ENA | Épine nasale antérieure | Extrémité antérieure du maxillaire | Tweed, Ricketts |
| ENP | Épine nasale postérieure | Extrémité postérieure du palais dur | Tweed |
| A | Point A | Point le plus déclive de la concavité antérieure du maxillaire | Tweed, Steiner, Ricketts |

**Mandibule**

| Point | Nom | Définition | Analyses |
|---|---|---|---|
| B | Point B | Point le plus déclive de la concavité antérieure de la mandibule | Tweed, Steiner |
| Pm | Suprapogonion | Point d'inflexion du contour antérieur de la symphyse entre B et Pog | Ricketts |
| Pog | Pogonion | Point le plus antérieur de la symphyse | Steiner, Ricketts |
| Gn | Gnathion | Point du contour symphysaire à égale distance de Pog et de Me | Steiner, Ricketts |
| Me | Menton | Point le plus inférieur de la symphyse | Tweed, Ricketts |
| D | Point D | Centre de la symphyse, au centre de sa base | Steiner |
| Go | Gonion | Point à égale distance du point le plus postérieur et du point le plus inférieur de l'angle goniaque | Steiner |
| Br | Point fictif | Sert uniquement à tracer la tangente au bord postérieur de la branche passant par Ar, pour mesurer la HFP | Tweed |
| Go′ | Point fictif | Sert uniquement à tracer la tangente au bord inférieur de la mandibule passant par Me (plan mandibulaire) | Tweed, Ricketts |

**Ramus (construction de Xi)**

| Point | Nom | Définition | Analyses |
|---|---|---|---|
| R1 | R1 | Point le plus profond de la concavité du bord antérieur du ramus, à mi-hauteur entre ses courbures supérieure et inférieure | Ricketts |
| R2 | R2 | Point du bord postérieur du ramus en regard de R1 (le point se place sur la parallèle à Francfort passant par R1) | Ricketts |
| R3 | R3 | Point le plus profond de l'échancrure sigmoïde | Ricketts |
| R4 | R4 | Point du bord inférieur de la mandibule à la verticale de R3 (le point se place sur la parallèle à PtV passant par R3) | Ricketts |

**Plan d'occlusion fonctionnel**

| Point | Nom | Définition | Analyses |
|---|---|---|---|
| OccP | Plan d'occlusion, point postérieur | Engrènement des 1res molaires | Tweed, Steiner |
| OccA | Plan d'occlusion, point antérieur | Milieu du recouvrement incisif | Tweed, Steiner |

**Dents**

| Point | Nom | Définition | Analyses |
|---|---|---|---|
| U1a | Incisive Mx, apex | Apex de l'incisive maxillaire | Tweed, Steiner |
| U1i | Incisive Mx, bord libre | Bord libre de l'incisive maxillaire | Tweed, Steiner |
| U1c | Incisive Mx, couronne | Point le plus vestibulaire de la couronne (I-NA) | Steiner |
| L1a | Incisive Md, apex | Apex de l'incisive mandibulaire | Tweed, Steiner, Ricketts |
| L1i | Incisive Md, bord libre | Bord libre de l'incisive mandibulaire | Tweed, Steiner, Ricketts |
| L1c | Incisive Md, couronne | Point le plus vestibulaire de la couronne (i-NB) | Steiner |
| U6d | 1re molaire Mx, face distale | Point le plus distal de la couronne de la 1re molaire maxillaire | Ricketts |

**Tissus mous**

| Point | Nom | Définition | Analyses |
|---|---|---|---|
| Cm | Columelle | Milieu du S formé par la columelle (ligne S de Steiner) | Steiner |
| Prn | Pronasale | Pointe du nez (ligne E de Ricketts) | Ricketts |
| Ls | Lèvre supérieure | Point le plus antérieur de la lèvre supérieure | Tweed, Steiner, Ricketts |
| Li | Lèvre inférieure | Point le plus antérieur de la lèvre inférieure | Tweed, Steiner, Ricketts |
| Pog′ | Pogonion cutané | Point le plus antérieur du menton cutané | Tweed, Steiner, Ricketts |

## Les mesures et leurs normes

Les normes sont celles du livre du  Pr Marie-José Boileau (*Orthodontie de l'enfant et du jeune adulte*). Une valeur sous la norme ou au-dessus est signalée dans la colonne d'interprétation.

### Analyse de Tweed

| Mesure | Définition | Norme |
|---|---|---|
| SNA | Angle S-Na-A | 82 ± 2° |
| SNB | Angle S-Na-B | 80 ± 2° |
| ANB | SNA - SNB | 2 ± 2° |
| AoBo | Distance entre les projections de A et B sur le plan d'occlusion fonctionnel, positive si Ao est en avant de Bo | 0 ± 2 mm |
| FMA | Francfort / plan mandibulaire | 25 ± 3° |
| HFAT | Na-Me | |
| HFAI | Distance de Me au plan bispinal | |
| HFP | Distance d'Ar au plan mandibulaire, le long de la tangente Ar-Br | |
| HFAI / HFAT | | < 55 % |
| HFP / HFAI | | 0,69 (0,65 à 0,75) |
| IMPA | Axe de l'incisive mandibulaire / plan mandibulaire | 85 à 92° |
| FMIA | 180° - FMA - IMPA | 68° |
| Occ / Francfort | Plan d'occlusion fonctionnel / Francfort | 10 ± 3° |
| I / i | Angle inter-incisif | 135 ± 5° |
| Angle Z | Francfort / tangente au Pog cutané et à la lèvre la plus protrusive | 78° (70 à 80°) |

**Difficulté cranio-faciale.** Pour chaque facteur, l'écart en dehors de l'intervalle est multiplié par le coefficient. Le total correspond à la part cranio-faciale de l'index de Merrifield, la difficulté dentaire, mesurée sur moulages, n'étant pas calculée.

| Facteur | Intervalle | Coefficient |
|---|---|---|
| FMA | 22 à 28° | 5 |
| HFP / HFAI | 0,65 à 0,75 | 3 par 0,01 |
| Occ / Francfort | 8 à 12° | 3 |
| ANB | 1 à 5° | 15 |
| SNB | 78 à 82° | 5 |
| Angle Z | 70 à 80° | 2 |

### Analyse de Steiner

| Mesure | Définition | Norme |
|---|---|---|
| SNA, SNB, ANB | Comme pour Tweed | 82 ± 2°, 80 ± 2°, 2 ± 2° |
| SND | Angle S-Na-D | 76 ± 2° |
| SE | Distance de S à E, projection d'Ar sur SN (à 12 ans) | 21 mm (19 à 23) |
| SL | Distance de S à L, projection de Pog sur SN (à 12 ans) | 51 mm (49 à 53) |
| GoGn / SN | Plan Go-Gn / SN | 32 ± 5° |
| I / NA | Axe de l'incisive maxillaire / NA | 22 ± 2° |
| I to NA | Distance du point le plus vestibulaire de la couronne de l'incisive maxillaire à NA | 4 ± 1 mm |
| i / NB | Axe de l'incisive mandibulaire / NB | 25 ± 2° |
| i to NB | Distance du point le plus vestibulaire de la couronne de l'incisive mandibulaire à NB | 4 ± 1 mm |
| Occ / SN | Plan d'occlusion fonctionnel / SN | 14 ± 3° |
| Pog to NB | Distance de Pog à NB | pas de norme |
| I / i | Angle inter-incisif | 131 ± 5° |
| Lèvres / ligne S | Distance de chaque lèvre à la ligne S (columelle - Pog cutané) | 0 ± 2 mm |

### Analyse de Ricketts (11 facteurs)

| Mesure | Définition | Norme à 9 ans | Variation avec l'âge |
|---|---|---|---|
| Axe facial | Ba-Na / Pt-Gn, angle postéro-inférieur | 90 ± 3° | aucune |
| Profondeur faciale | Francfort / Na-Pog | 87 ± 3° | + 1° tous les 3 ans |
| Angle du plan mandibulaire | Francfort / Me-Go′ | 26 ± 4° | - 1° tous les 3 ans |
| Hauteur faciale inférieure | Angle ENA-Xi-Pm | 47 ± 4° | aucune |
| Arc mandibulaire | Dc-Xi / Xi-Pm | 26 ± 4° | + 0,5° par an |
| Hauteur faciale totale | Na-Ba / Xi-Pm | 60 ± 3° | aucune |
| Convexité | Distance de A à Na-Pog | 2 ± 2 mm | - 1 mm tous les 3 ans |
| i to A-Pog | Distance du bord libre de l'incisive mandibulaire à A-Pog | 1 ± 3 mm | aucune |
| i / A-Pog | Axe de l'incisive mandibulaire / A-Pog | 22 ± 4° | aucune |
| Angle de Mc Horris | Axe de l'incisive mandibulaire / droite condylion-bord libre | 90 ± 5° | aucune |
| 6 / PtV | Distance de PtV à la face distale de la 1re molaire maxillaire | âge + 3 mm, ± 2 | selon l'âge |
| Lèvre supérieure / ligne E | Distance à la ligne E (pronasale - Pog cutané) | - 1 ± 2 mm | aucune |
| Lèvre inférieure / ligne E | Distance à la ligne E | 0 ± 2 mm | aucune |

**Indice VERT.** Il fait la moyenne des écarts à la norme, exprimés en écarts-types, de cinq facteurs : axe facial, profondeur faciale, angle du plan mandibulaire (signe inversé), hauteur faciale inférieure (signe inversé) et arc mandibulaire. Une valeur inférieure ou égale à - 0,5 oriente vers un type dolichofacial, une valeur comprise entre - 0,5 et + 0,5 vers un type mésofacial, une valeur supérieure ou égale à + 0,5 vers un type brachyfacial. Au-delà de ± 1,5, le type est dit sévère.

## Conventions de calcul

Les distances aux droites (I to NA, i to NB, Pog to NB, convexité, i to A-Pog, lèvres) sont positives lorsque le point est en avant de la droite et négatives lorsqu'il est en arrière. AoBo est positif lorsque Ao est en avant de Bo. Le plan d'occlusion utilisé est le plan d'occlusion fonctionnel, passant par l'engrènement des premières molaires et le milieu du recouvrement incisif.

## Téléradiographies

Aucune téléradiographie n'est fournie avec l'application. Pour s'entraîner, il est possible de télécharger des téléradiographies de profil sur le site de l'AAOF Craniofacial Growth Legacy Collection (aaoflegacycollection.org). L'image doit comporter une règle radiographique ou un repère de longueur connue pour permettre la mise à l'échelle.

## Avertissement

Cette application est un outil pédagogique d'aide à l'analyse céphalométrique. Elle ne se substitue pas au jugement clinique du praticien. La précision des résultats dépend directement de la qualité du placement des points et de la mise à l'échelle.

## Auteur et licence

© 2026 Dr Anaïs Cavaré. Application développée avec l'assistance de Claude (Anthropic), modèle Fable 1.

Diffusée sous licence [Creative Commons BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.fr) : usage libre et gratuit, avec mention de l'auteur. L'utilisation commerciale est interdite, et toute version modifiée doit être diffusée sous la même licence. Le texte complet de la licence figure dans le fichier `LICENSE`.
