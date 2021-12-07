<head>
  <link rel=«stylesheet» type="text/css" href=«reponse.css»>
</head>
<body>
  <h1>Compte rendu TD 3 WEB :</h1>
  <h2>Exercice 1 :</h2>
  <ol>
    <blockquote>
      Dessinez l'architecture de page par défaut (version faite lors du dernier TP => pour un écran supérieur à 800px) et l'architecture qu'aurait cette même page, si on devait l'adapter à un écran pour un dispositif plus petit, comme une tablette dont la largeur peut être inférieure à 800 pixels.
      <ul>
        <li>Voici une vidéo montrant à quoi ressemble cette adaptation.</li>
        <li>Identifiez les boîtes qui devront changer de style d'affichage pour parvenir à la nouvelle architecture;</li>
        <li>Précisez/expliquez quelles modifications ces boîtes doivent subir. Ne donnez aucun code pour répondre à cet exercice.</li>
      </ul>
    </blockquote>
    <li>Les boites qui devront changer de style sont les 3 boites <article class=  « cols »>, on va devoir linéariser les 3 colonnes afin de n’en reformer qu’un seule en leur rendant leur largeur afin qu’elle occupe la largeur de la section.</li>
      <br>
      <blockquote>
        Maintenant, essayons d'implémenter cette adaptation "tablette". Ajoutez à l’intérieur du fichier CSS des règles qui ne seront appliquées que si la largeur du dispositif de lecture est inférieure ou égale à 800px (ce qui peut-être le cas de petites tablettes).
        <ul>
          <li>Quel media query devez-vous utiliser ?</li>
          <li>Faites en sorte que votre page ne comporte que 2 colonnes (sans toucher au fichier HTML). On veut une colonne pour le flux twitter à droite, et une 2ème colonne avec le contenu principal à gauche;</li>
          <li>La boîte du contenu principal ne possède qu'une seule colonne (i.e. les trois colonnes internes doivent être « linéarisées »).</li>
        </ul>
      </blockquote>
    <li>@media screen and (max-width : 800px) <br>
        Le reste de la question est dans le css.
    </li>
  </ol>
  <h2>Exercice 2 :</h2>
  <ol>
    <blockquote>
      Ajoutez dans le fichier HTML de l'exercice 1, un media query qui appliquera les règles CSS d’un fichier smartphone.css si la taille de l’écran est inférieure ou égale à 600px. Vous devez créer le fichier smartphone.css à partir de rien.
      <ol>
        <li>Comment insère-t-on ce media query dans le fichier HTML ?</li>
        <li>
          Dessinez l'architecture de la page adaptée aux tablettes et l'architecture de page adaptée aux petits écrans.
          <ul>
            <li>Voici une vidéo montrant à quoi ressemble cette adaptation.</li>
            <li>Identifiez les boîtes qui devront changer de style d'affichage pour parvenir à la nouvelle architecture</li>
            <li>Précisez/expliquez quelles modifications ces boîtes doivent subir. Ne donnez aucun code pour répondre à cet exercice.</li>
          </ul>
        </li>
      </ol>
    </blockquote>
    <li>&lt;link rel=«stylesheet» type=«text/css» media=«screen and (max-width : 600px)» href=«smartphone.css»&gt;</li>
    <li>En dessous de 600px, le twitterfeed repasse en dessous de la colonne principale et le menu est caché un bouton apparait afin de le remplacer en prenant moins de place.</li>
    <li><strong>Bonus : </strong><br>Si le sous menu était sur la case 3, pour le position relative, le top serait à -20px et non à -42px parce que l'on doit le descendre de 18px pour descendre d'une case et encore de 4px à cause de la double bordure.</li>
  </ol>
</body>
