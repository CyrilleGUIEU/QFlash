# QFlash

## Un outil pour élaborer des séries de question flash

### Le principe

QFlash utilise le langage Latex pour décrire les questions et leurs solutions. Le principe de fonctionnement consiste à utiliser un seul script pour générer le fichier PDF de passation en classe et celui de bilan qui contiendra les corrections.

Voici un exemple: [Source latex](https://github.com/CyrilleGUIEU/QFlash/blob/master/Exemples/Script%20de%20mise%20au%20point.tex) -> [PDF de passation](https://github.com/CyrilleGUIEU/QFlash/blob/master/Exemples/QuestionsFlash.pdf) + [PDF de correction](https://github.com/CyrilleGUIEU/QFlash/blob/master/Exemples/QuestionsFlashCorrection.pdf)

### Prérequis

Quelques rudiments de langage Latex sont nécessaires pour utiliser cet outil. 

Les logiciels nécessaires au fonctionnement de QFlash sont les suivants:

**Pour la conception des questions/réponses:**

* Une distribution Latex (par exemple [Miktex](miktex.org))
* Un éditeur de code Latex (par exemple [TexMaker](https://www.xm1math.net/texmaker/index_fr.html))

**Pour la lecture en classe ou à partir d'un ENT:**

* Un lecteur PDF qui autorise le défilement automatique (par exemple [Acrobat Reader](https://get.adobe.com/fr/reader/), attention aux logiciels facultatifs qui viennent par défaut avec ce logiciel, vous n'êtes pas obligés de les accepter !)

### Premier pas

1. Compiler l'exemple donné:
* Téléchager ce dépôt
* Depuis un éditeur Latex, ouvrir le fichier "Exemples/Script de mise au point.tex"
* Compiler ce script en utilisant * *pdflatex* *
* Tester le PDF obtenu
* Recommencer en modifiant les variables **timer** et **correction** situées au début du script

2. Créer votre propre questionnaire:
* Dupliquer le dossier "Exemples" en restant dans le même dossier
* Modifier le nom de ce dossier en fonction de votre projet
* Modifier et renommer le "Script de mise au point" en fonction de vos besoins

**Note:** Il est nécessaire le fichier "qflash.tex" soit trouvé par le fichier tex de définition des questions/réponses. Cela peut ne pas être le cas si vous déplacez le dossier dupliqué.
