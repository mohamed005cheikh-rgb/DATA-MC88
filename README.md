<div align="center">

# 🏭 Data Factory MC88

**Des jeux de données réalistes, en quelques secondes.**

</div>

---

## 👋 Bienvenue

Data Factory est un générateur de données de test qui tient dans une seule page.

Vous choisissez un secteur, une culture de noms, un nombre de lignes — et l'outil vous fabrique un jeu de données crédible, prêt à être utilisé. Pour tester une application, pratiquer le nettoyage de données, préparer une démonstration, ou simplement remplir une base de développement avec quelque chose qui ressemble à la réalité.

Tout se passe **dans votre navigateur**. Aucun serveur, aucun compte, aucune donnée envoyée. Vous générez, vous exportez, vous fermez.

Et si vous voulez voir comment vos outils se comportent face à des données imparfaites, un mode « données sales » est là pour ça — valeurs manquantes, fautes de frappe, formats incohérents, valeurs aberrantes. Comme dans la vraie vie.

---

## 📸 Un aperçu

<div align="center">
  <img src="https://github.com/mohamed005cheikh-rgb/data-mc88/raw/main/images/Sc1.png" alt="Configuration et prévisualisation" width="100%" />
</div>

<br />

<div align="center">
  <img src="https://github.com/mohamed005cheikh-rgb/data-mc88/raw/main/images/Sc2.png" alt="Exportation dans plusieurs formats" width="100%" />
</div>

<br />

<div align="center">
  <img src="https://github.com/mohamed005cheikh-rgb/data-mc88/raw/main/images/Sr1.gif" alt="Générer un jeu de données en un clic" width="100%" />
</div>

<br />

<div align="center">
  <img src="https://github.com/mohamed005cheikh-rgb/data-mc88/raw/main/images/Sr2.gif" alt="Activer le mode données sales" width="100%" />
</div>

---

## ✨ Ce que vous trouverez

**Huit secteurs, chacun avec sa logique propre.**  
Retail et e-commerce, banque et finance, santé, aviation, logistique, éducation, ressources humaines, profils personnels. Chaque secteur a ses propres colonnes — commandes et clients pour le retail, transactions et statuts pour la banque, patients et diagnostics pour la santé. Les données ne sont pas juste aléatoires : elles suivent la structure du métier.

**Neuf cultures pour les noms et les lieux.**  
Arabes, français, anglais, indiens, canadiens, australiens, sud-africains, allemands, espagnols. Chaque culture apporte ses prénoms, ses noms de famille, ses villes, et même ses formats de numéro de téléphone. Vous pouvez ainsi produire des jeux de données qui ressemblent vraiment à ce que vous verriez dans un pays donné.

**De 50 à 50 000 lignes.**  
Des petits échantillons pour tester vite, ou de gros volumes pour éprouver la robustesse de votre code. Le choix se fait en un clic, ou en saisissant un nombre précis.

**Une graine, pour des résultats reproductibles.**  
Entrez n'importe quelle valeur dans le champ « Seed », et vous obtiendrez **exactement le même jeu de données** à chaque génération. Très utile pour reproduire un bug, partager un exemple avec un collègue, ou faire une démonstration stable. Laissez vide, et chaque génération sera différente.

**Un mode « données sales » pour être réaliste.**  
Vous voulez voir comment votre application se comporte face à des données imparfaites ? Cochez une case, réglez le pourcentage, et l'outil injecte :
- des valeurs manquantes,
- des fautes de frappe,
- des dates aux formats incohérents,
- des valeurs aberrantes (nombres multipliés par 50 à 150),
- des noms de colonnes irréguliers,
- et parfois même des lignes dupliquées.

Comme dans un vrai fichier qui a passé trop de temps entre les mains de trop de gens.

**Six formats d'export.**  
CSV, Excel, JSON, SQL, XML, Markdown. Pour chaque format, le fichier se télécharge immédiatement, avec les bons types de données préservés. Et pour un usage rapide, un bouton **Copier** met les 200 premières lignes au format TSV, prêtes à coller dans Excel ou Google Sheets.

**Un aperçu immédiat.**  
Les vingt premières lignes s'affichent dans un tableau — avec les en-têtes figés pour un défilement confortable, les valeurs manquantes en gris, et les valeurs aberrantes en rouge. Un coup d'œil suffit pour vérifier que le jeu de données vous convient.

**Deux ambiances.**  
Un thème sombre et un thème clair, d'un clic. Votre choix est conservé pour la prochaine visite.

---

## 🧭 Comment ça marche

Cinq gestes, toujours les mêmes.

**1. Choisissez un secteur.**  
C'est lui qui détermine les colonnes du jeu de données. Chaque secteur a sa structure.

**2. Choisissez une culture.**  
Les noms, les villes et les formats de téléphone suivront cette culture.

**3. Définissez le nombre de lignes.**  
De 50 à 50 000. La prévisualisation reste légère — mais l'exportation produira bien tout ce que vous avez demandé.

**4. (Optionnel) Fixez une graine.**  
Si vous voulez reproduire exactement les mêmes données plus tard, entrez une valeur dans le champ *Seed*.

**5. Générez, puis exportez.**  
Un clic sur *Generate*, un coup d'œil au tableau, et vous choisissez le format de sortie. Le fichier se télécharge automatiquement.

Rien n'est définitif tant que vous n'avez pas cliqué sur un bouton d'export — vous pouvez régénérer, changer de secteur, essayer une autre graine, autant de fois que vous voulez.

---

## 🛠️ Petits coups de main

**Le bouton *Generate* ne répond pas ?**  
Vérifiez que le champ « Row Count » contient bien un nombre valide, entre 1 et 50 000. Si vous avez tapé autre chose que des chiffres, l'outil refuse poliment.

**Rien ne se télécharge ?**  
La plupart du temps, aucun jeu de données n'a été généré. Cliquez d'abord sur *Generate*, puis sur le format souhaité. Si le problème persiste, vérifiez que votre navigateur autorise les téléchargements multiples.

**Le fichier Excel refuse de s'ouvrir ?**  
La bibliothèque qui produit le `.xlsx` se charge au premier lancement. Vérifiez votre connexion, rechargez la page, et attendez que tout soit en place avant de générer.

**Les données sont identiques à chaque fois ?**  
Regardez le champ « Seed ». S'il contient une valeur, elle fixe le hasard — c'est le comportement attendu. Videz le champ pour retrouver des données différentes à chaque génération.

**La page ralentit vers 50 000 lignes ?**  
C'est le maximum prévu, et c'est un cap réel. La prévisualisation n'affiche que vingt lignes, mais l'exportation traite tout. Si vous travaillez sur une machine modeste, testez avec 2 000 ou 5 000 lignes — vous verrez souvent la même chose.

**Le mode « données sales » ne change rien ?**  
Le curseur est probablement resté à 5 %, le minimum. Montez à 30 ou 50 % pour voir la différence — les anomalies deviennent alors visibles dès la prévisualisation.

**Le bouton *Copy* ne copie rien ?**  
Vérifiez qu'un jeu de données existe, puis autorisez l'accès au presse-papiers dans votre navigateur. En dernier recours, l'exportation CSV fait la même chose.

**Les noms ne correspondent pas à la culture choisie ?**  
La culture a changé **après** la génération — le tableau affiché est encore l'ancien. Régénérez pour voir la nouvelle culture appliquée.

---

<div align="center">

### 📞 Une question, une idée ?

[![Email](https://img.shields.io/badge/Email-mohamed005cheikh@gmail.com-d14836?style=flat-square&logo=gmail&logoColor=white)](mailto:mohamed005cheikh@gmail.com)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-+222_30_72_64_75-25D366?style=flat-square&logo=whatsapp&logoColor=white)](https://wa.me/22230726475)

<br />

*Bonnes générations.*

<sub>© 2026 Mohamed Cheikh — MC88</sub>

</div>
