# Guide d’annotations : scènes d’accouchement dans la littérature

Cette page se veut présenter la méthodologie à l'œuvre dans le cadre de l’annotation manuelle des scènes d’accouchement dans la littérature.

## Logiciel d’annotation : 

Nous veillerons à utiliser le logiciel d’annotation INCEpTION.
C'est un outil open-source ; la documentation française et anglaise est accessible en fin de document.

_____

# Étapes de paramétrage INCEpTION : 

- ## Création de layer (couche) 

La layer est la couche/catégorie générale d’annotation. 

### > **scene\_accouchement (granularité scène entière)**  
  - span  
  - Annotation des scènes d'accouchements : granularité niveau phrase granularity : sentence-level  
  - **overlap** : any

  ### > **phase\_accouchement**  
- span  
- annotation de l’accouchement, dans les scènes d'accouchement  
- granularity : token-level  
- overlap : any  
    - **features :**   
	      - Phases\_accouchement  
	      - **type** : primitive: String  
	      - Annotation/identification des différentes phases de l'accouchement  
	      - **tagset** : Accouchement\_phases  
	      - **editor** **type** : combo-box

### > **personnage**   
- span  
- Personnages actrices/acteurs dans les scènes d'accouchements  
- **granularity** : token-level  
- **overlap** : any  
    - **features :**   
	      - Which\_character  
	      - **type** : primitive: String  
	      - Quel personnage en présence ?  
	      - **tagset** : Wich\_character\_here  
	      - **editor type** : combo-box


### > **grossesse (granularité scène entière)**  
  -  span  
  - Annotation des scènes d'accouchements : granularité niveau phrase  
  - granularity : sentence-level  
  - **overlap** : any


### > **complication**  
  - span  
  - Phases de complication liée aux scènes d'accouchements  
  - granularity : token-level  
  - **overlap** : any



________


- ## Création de tagsets :

Les tagsets permettent d’annoter plus précisément ; ils spécifient un layer. 

### > **Accouchement\_phases**  
  - fra  
  - différentes phases de l'accouchement : 
  *Liste des types choisis* :

- **travail**

Le travail désigne l'ensemble des phénomènes qui permettent l'expulsion du bébé. C'est la phase active qui commence lorsque les contractions deviennent régulières, intenses et rapprochées.  
Le début du travail, lors d’un accouchement par voie basse, est le plus souvent spontané. Il est marqué par la survenue de contractions qui, au fil des heures, deviendront de plus en plus intenses et régulières, associées parfois à la rupture de la poche des eaux.

- **dilatation(contraction)**

Pour la naissance d’un premier bébé (on dit que la maman est primipare), cette phase de dilatation du col de l'utérus dure environ huit heures. Elle ne dure plus que quatre heures en moyenne, chez une femme multipare ayant déjà eu au moins un enfant.

Les contractions, d’abord brèves et espacées (toutes les dix minutes) se rapprochent (cinq minutes, puis moins), deviennent régulières, plus intenses et douloureuses. Sous l’effet des contractions, le col de l'utérus s’ouvre très progressivement.  
’est durant cette phase que vous vous rendez à la maternité. À l'arrivée, vous êtes prise en charge et examinée par la sage-femme ou l’obstétricien. Si le travail est suffisamment avancé, vous êtes installée en salle de travail.

- **expulsion (naissance)**

La phase d’expulsion (naissance) du bébé est relativement courte et ne dure qu’une trentaine de minutes environ.  
Lorsque le col de l'utérus est ouvert complètement (la dilatation du col atteint alors 10 cm) et que la tête du bébé (la partie la plus large) est bien engagée dans le bassin, la sage-femme ou l’obstétricien vous demande de pousser. Ces poussées, lors des contractions, permettent l’expulsion du bébé.  
Une fois la tête sortie, le corps du bébé glisse sans difficulté.  
Votre bébé est né \! La sage-femme coupe le cordon ombilical, vérifie la bonne vitalité de votre bébé et pose votre enfant contre vous.

- **délivrance**

L’accouchement ne s’achève réellement que vingt à trente minutes plus tard. Sous l’effet de nouvelles contractions utérines, la maman expulse le . C'est ce qu’on appelle la délivrance.



### > **Wich\_character\_here**  
  - fra  
  - Différents personnages en présence lors de l'accouchement :  
    - Accouchée  
    - Accouchant F  
    - Accouchant H  
    - Témoin  
    - *Géniteur ?*

### > **Intervention médicale
  - fra  
  - Différentes interventions médicales
	  - *Types d'interventions à préciser*

### > **which\_complication**  
  - fra  
  - Différentes complications liées aux phases d’accouchements
	  - *Types de complications à préciser



____

## Documentation consultée : 

- **user guide INCEpTION eng** : https://inception-project.github.io/releases/39.6/docs/user-guide.html
- **user guide INCEpTION fra** :  [https://corli.huma-num.fr/wp-content/uploads/2022/05/Fiche-8-Cre%CC%81ation-dune-couche-dannotation.pdf](https://corli.huma-num.fr/wp-content/uploads/2022/05/Fiche-8-Cre%CC%81ation-dune-couche-dannotation.pdf)  
- **user guide INCEpTION fra** : [https://corli.huma-num.fr/fr/faq/comment-utiliser-la-plateforme-inception/](https://corli.huma-num.fr/fr/faq/comment-utiliser-la-plateforme-inception/)  
- **Phases** **accouchement** : [https://www.ameli.fr/assure/sante/devenir-parent/accouchement-nouveau-ne-et-retour-la-maison/accouchement](https://www.ameli.fr/assure/sante/devenir-parent/accouchement-nouveau-ne-et-retour-la-maison/accouchement)  


