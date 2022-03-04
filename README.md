# sutom-helper
<h1>Un programme permettant d'affiner la recherche du mot correct pour le SUTOM</h1>

Lancer en utilisant python et en utilisant la syntaxe suivante : </br>
<code>python main.py longueurDuMot LettresOrdonnes LettreAvecPositionInconnue LettresAbsentesDuMot</code>
Utiliser un astérisque *  pour représenter les caractères inconnus
exemple 1 : <code>python main.py 5 MO**S * *</code>
Ici mot de 5 lettres commençant par MO et finissant par S et donc on ne connaît pas d'autres lettres présentes et dont on ne connaît pas de lettres non présentes.

exemple 2 : <code>python main.py 6 MA**** N BCDP</code></br>
Ici le mot fait 6 lettres, on sait qu'il commence par MA, on sait qu'il contient N et I mais on ne sait pas où et on sait qu'il ne contient PAS les lettres B,C,D,P

Le programme retourne alors les mots correspondant aux informations entrées, elles sont classées par leur ordre d'apparition dans le dictionnaire utilisé</br>

['magnai', 'mainte', 'maints', 'maison', 'malien', 'maline', 'malins', 'maniai', 'manias', 'maniat', 'maniee', 'manier', 'manies', 'maniez', 'manifs', 'manoir', 'marina', 'marine', 'marins', 'marlin', 'marnai', 'martin', 'matina', 'matine', 'matins']
<strong>Plus les informations entrées sont précises moins de mots seront trouvées et les solutions données permettront alors de trouver la solution plus facilement.</strong>

Mots récupéres : https://sutom.nocle.fr/js/mots/listeMotsProposables.js
