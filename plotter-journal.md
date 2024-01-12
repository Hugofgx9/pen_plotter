Plotter journal

01/12
J'ai trouvé plusieurs tutoriels et ressources qui proposent des méthodes qui me semblent accessible. Cela demande de l'impression 3d, de l'arduino, un peu de mécanique, un peu d'elec et d'informatique. Je vais regarder un peu plus précisément les différents tutoriels pour savoir vers lequel me diriger et commander le materiel rapidement.

02/12
La conception en T (ou en +) semble être la plus répandu puisqu'elle offre la meilleur rapport qualité/place. Je peux utiliser des nom de pieces carrées ou des tiges en métal ? Lequel et les moins bruyant ?
04/12
Le but est évidemment dépenser le moins d'argent possible pour la v1, quitte à acheter des composants plus pertinents pour une futur upgrade. J'ai réussi à récupérer 1 arduino uno, 2 stepper nema 17 (avec bcp plus de couple que nécessaire) et 2 motor driver au travail. Les tutoriels que j'ai vu utilisent tous un shield CNC sur lequel ils mettent des driver moteurs minuscules et qui ne correspondent pas à ceux que j'ai récupéré. Je vais essayer d'adapter leur projet avec mes driver arduino, si c'est trop complexe, je commanderais leurs driver. De plus, je doute que leurs tout petits driver suffisent à envoyer suffisamment d'intensité dans mes moteurs beaucoup plus puissants.
Il me semble important de faire un planning, pour planifier mon organisation. La partie logicielle semble plus compliquée que ce que je pensais et il faut prévoir du temps sur cette partie également, peut-être au début pour être certain que mon hardware sera compatible.
13/12
J'ai commandé un fer à souder, un multi-mètre, et des fils arduino.
Les système de profilés alus avec des fentes se trouve sous le nom de v-slot ou c-beam. Il existe des plateaux compatibles que l'on trouve sous le même nom. 
Il existe plusieurs systèmes pour propager le déplacement du moteur au plateau : courroie caoutchouc (belt) ou vis sans fin (lead screw). Comparaison : https://www.pbclinear.com/blog/2020/february/lead-screw-or-belt-drives  . La courroie semble être plus intéressante car elle permet des déplacement plus rapide mais peut être plus compliquée à rendre précise. Les systèmes à vise sont plus  destinées à des mouvements lent et très précis, comme l'impression 3d.
La courroie et les poulie doivent être compatibles. Pour l'instant, je pense partir sur des poulie GT2 20 dents pour axe 5mm, compatible avec des courroies GT2 6mm.
Voilà un schéma à la main reprenant les différents éléments de conception. 
![IMG\_7811.jpeg](files/img_7811.jpeg)    

14/12
Aujourd'hui, je m'attaque à la conception et impression 3d. J'ai déjà approché la conception assistée par ordinateur (CAO) lors de plusieurs petits projets perso, mais qui sont restés à des stades d'ébauches dans mon ordinateurs. Je n'ai jamais été jusqu'à l'impression 3d. Le but de cette journée est d'appréhender la pipeline conception/impression, pour estimer le temps que ces taches peuvent me prendre et la simplicité (ou difficulté) pour passer du fichier numérique à l'objet réel, la solidité de celui ci, si des marges sont nécessaires, …
Choix du logiciel de CAO
Ayant déjà eu qqs projets de CAO, je connais les outils possibles. Les outils "pro" autodesk, solidworks, catia,… L'alternative libre Freecad, le plugin sketcherCAD de blender. Le plugin de blender est très prometteur mais il manque quelques fonctionnalités essentielles pour l'instant. Si le développement avance vite ça deviendra la meilleure option. Les outils pro sont très/trop chères pour mon usage, il existe des offre étudiantes qui sont souvent payantes, limitantes et je préfère ne pas être dépédant de logiciels payant pour ma pratique futur. FreeCAD a un interface un peu daté/chargé mais est très complet et pratique une fois pris en main, en plus le logiciel est libre et gratuit, je pars donc là dessus.
Je modélise une pièce simple de mon plotter, un support pour les profilés. Ça me prend environ 1h30, puis 30min pour setup l'impression. L'impression dure 1h20.
L'impression est bonne, une partie est un peu déformée, je pense que ça vient d'un soucie de température de buse pendant l'impression. Je n'ai pas pu mesurer avec un pied à coulisse mais j'ai l'impression que l'épaisseur du fil nécessite d'ajouter environ 1mm de marge par bord
   
29/12
J'ai beaucoup avancé sur la conception 3d ces derniers jours. Finalement je suis revenu sur Freecad, il manque une fonctionnalité sur le sketcher de blender, j'ai essayé de modifier un peu le plugin mais je ne comprends pas assez l'api de blender pour être à l'aise et y passer trop de temps. Mais cela m'a permis de plonger dans la création de plugin blender, que je garde en tête pour un prochain projet :). 
Coté conception les 2 bouts de l'axes principal sont presque finis. Je me heurte actuellement à des reflexion sur le facilité d'accessibilité et de réglage des pièces. L'un des gros point d'interrogation que j'ai est la disposition et fixation du moteur. Je doute que 2 vis dans l'impression 3d soient suffisantes pour supporter la force du déplacement.   
03/01
J'ai appelé Yann, la personne qui s'occupe de la conception et des impressions 3d chez scale, pour avoir son avis sur ma premiere version. Il m'a confirmé que ma conception n'était pas bonne et ne soutiendrai pas la force du moteur. Selon lui, le moteur doit être une partie fixe et la tension de la courroie s'ajuster avec des petits modules fais pour. Il m'a donné plusieurs système qui existent et j'ai trouvé des modèles sur Thingiverse.
Je vais les adapter à ma conception et modifier l'emplacement et la fixation du moteur.
   
[Belt tension thingiverse](belt-tension-thingiverse.md)    
08/01
J'ai fini de modéliser cette deuxième version, en prenant en compte les retours de Yann. Cela m'a permis d'apprendre beaucoup plus en profondeur freecad, pour la création de formes complexes, d'engrenages, de vis et de courbes. Selon Yann, mes 2 supports peuvent être compliqué à imprimer, je lancerais les impressions dès lundi en arrivant aux Gobelins pour adapter si besoin. Il faut également que je lance la commande de matériel.
   
