# The Honest Marketing Robot
* begin : un robot te propose de gagner 100€
* end: tu ouvres un compte et reçois 100€
* failure: tu refuses d'ouvrir un compte

## intro
_Tu marches dans la rue, pas loin de chez toi, et tu remarques un robot qui attend là, posé. Il a un écran sur la tête, simulant une paire d'yeux style cartoon_

Bonjour humain, souhaiterais-tu gagner 100€ ? 78% des humains interrogés ont répondu par l'affirmative.

* ok, que je dois-je faire ? -> game_accepted
* 100€, pour de vrai ? -> irl_money
* non merci, pas intéressé. -> are_you_sure

## game_accepted
_L'écran du robot passe par toutes les couleurs de l'arc-en-ciel, il a l'air très emballé par la réponse reçue_

C'est vrai, tu veux vraiment ? Oh merci humain ! Beaucoup m'ont dit non [ce matin/cet après-mid/ce soir]. Mon module émotionnel tournait en mode dépression depuis 1 heure.

* oui je veux vraiment / y'a pas de quoi ->  instructions
* C'est quoi le module émotionnel ? -> TODO
* finalement non -> are_you_sure

## irl_money
_Le robot a l'air de ... plisser les yeux_

Bien sûr que je te les filerai pour de vrai. A une condition, tu dois ouvrir un compte en banque chez mabanquenligne.com pour que je puisse te les y déposer.

* comment ouvrir un compte ? -> open_account
* pourquoi mabanquenligne.com ?

## are_you_sure
TODO

## instructions
