# Côté front-end

### Nous avons fait 2 Landing Pages :
+ [Une destinée aux **professionnels en reconversion**](https://landing-thehackingproject.herokuapp.com/)
+ [Une pour les **entrepreneurs en recherche de CTO**.](https://thp-landing-entrepreneur.herokuapp.com/)

Pour cela nous avons téléchargé deux thèmes différents sur [start Bootstrap](https://startbootstrap.com/) et nous les avons implémentés dans nos applications Rails.

Nous avons réfléchis au wording qui correspond **exactement** à nos segments, après avoir défini les cibles, sur la base des profils de la session actuelle.
Nous avons aussi sélectionné en fonction des landing et de la cible de jolies photos libre de droits sur [unsplash](https://unsplash.com) 
Nous avons établi qu'il serait de bon ton de donner quelque chose en retour des emails qu'ils allaient nous soumettre, ce qui se fait souvent c'est de recevoir un livre blanc, un pdf pour donner un avant goût. Dans notre cas, nous pensons que le projet d'une journée type (reproduire la page de Google par exemple) serait pertinente pour nos visiteurs, c'est pourquoi nous avons respectivement argumenté :
>"Recevez dès maintenant l'exercice d'une journée type" 
> **Ça m'intéresse !**

et 
>3 mois pour coder ton produit tech !
>**Voir une journée type**

Puis le bouton déclenche une pop-up dans laquelle on lui explique qu'il recevra l'extrait par email. :boom:

Enfin, nous avons mis [Olark](https://www.olark.com) pour que les visiteurs puissent directement interragir avec ceux qui gère la landing pageTHP, au cas où ils ont des questions..

Il n'y a **aucun** lien autre que le submit pour réceptionner les emails.


# Côté back-end :

Pour chaque app, nous avons pluggé **un compte MailChimp** qui récupère les emails que l'utilisateur rentre dans l'input contre un extrait du programme de THP (la journée HTML/CSS pour refaire la page de Google par exemple).

On a aussi ajouté **Google Analytics** afin de pouvoir analyser nos campagnes de communication (cela est couplé à l'outil Google Analytics URL Builder, ainsi que BitLy pour raccourci les URLs).


## Stratégie d'acquisition 
Une de nos deux cibles est les fondateurs ou futur fondateurs de startup tech qui n'ont pas de compétences techniques.
Beaucoup de ces profils sont plutôt business et cherchent un CTO avec qui s'associer pour lancer leur projet mais ont du mal à les trouver et les convaincre.
_Il faut dire que les développeurs ne manquent pas de propositions et il est pas facile de les convaincre !_

Du coup, on a voulu attirer un max de profils comme ça qui seraient susceptibles de devenir leur propre CTO en faisant THP.
En effet, Anthony Amar en est la preuve vivante : il fait THP pour acquérir des connaissances et développer son projet pendant THP.
#### La stratégie est la suivante:
* On a laissé des annonces sur les groupes facebook de startuppeurs en ce faisant passer pour un jeune developpeur qui est pret à s'associer sur un projet et prendre la casquette de CTO
* Dans l'annonce, on l'invite à nous contacter par mail en spécifiant une nouvelle adresse gmail
* On lance notre bot que l'on a développé sur Ruby pour l'occasion (cf. les services)
* Le bot va récupérer tout les emails des expediteurs, les ajouter dans la liste mailchimp
* Et leur répondre avec un mail automatique qui explique qu'il peut lancer sa startup en devenant son propre CTO avec THP. L'email envoi également le lien de la landing page :boom: :boom: 