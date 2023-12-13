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