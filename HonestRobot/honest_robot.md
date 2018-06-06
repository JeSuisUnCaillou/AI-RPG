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

Oh yessss, merci humain ! Beaucoup m'ont dit non [ce matin/cet après-mid/ce soir]. Mon module émotionnel tournait en mode dépression depuis 1 heure.

* oui je veux vraiment / y'a pas de quoi ->  instructions
* C'est quoi le module émotionnel ? -> TODO
* finalement non -> are_you_sure

## irl_money
_Le robot a l'air de ... plisser les yeux._

Bien sûr que je te les filerai pour de vrai. A une condition, tu devras ouvrir un compte en banque chez mabanquenligne pour que je puisse te les y déposer.

* comment ouvrir un compte ? -> open_account

## are_you_sure
TODO

## instructions
Alors, pour ouvrir un compte, tu dois escalader l'Evrest à reculons en jouant de la cornemuse tout en écrivant une pièce de théatre en 8 actes sur l'esclavage en Grèce antique. Deal ?

_Une inscription clignotante a remplaçé les yeux du robot. Il y est écrit 'Blague', 'Humour', 'Drôle'_

* non mais sérieusement, là -> serious_instructions
* yeah, deal ! -> serious_instructions (absurd_deal_accepted: true)

## serious_instructions
absurd_deal_accepted: true > Non mais je déconnais là. T'allais pas sérieusement jouer de la CORNEMUSE ?!

absurd_deal_accepted: false > Ok, j'avoue mon module d'humour est bloqué sur 'absurde' depuis 2 jours.

En vrai, t'as juste à me fournir une pièce d'identité. Genre une photo de ta carte d'identité ou permis de conduire avec ton smartphone suffit.

Basique... Simple.

* bouton photo/upload carte recto/verso -> verify_id_data
* document non reconnu -> TODO

## verify_id_data
_Un symbole de carte d'identité orange s'affiche sur son torse_

_Le robot a des soubresauts comme si il était en train de se marrer_

Haha, la tête ! Hum, pardon. Je ne suis pas censé me moquer des clients. Peux-tu vérifier les informations que j'ai lues ? Je ne suis pas tout à fait sûr de savoir correctement lire...

* bouton 'vérifier les informations' (voir marvel d'Henri avec les swipe left/right) -> i_lied

## i_lied
_Un symbole de carte d'identité vert s'affiche sur son torse_

Okay ! Merci pour ces confirmations. Bon je dois t'avouer quelque chose... En vrai j'ai besoin d'un deuxième document. C'est un justificatif de domicile. Genre une facture EDF, ou de téléphone mobile.

Promesse de cyber-scout, c'est le dernier truc que je te demande ! Après ça, j'touvre le compte et à toi les 100 balles.

* bouton photo/upload justificatif domocile -> verify_domicile_data
* document non reconnu -> TODO

## verify_domicile_data
_Un symbole de maison orange s'affiche sur son torse_

Tu peux vérifier ce que j'ai lu dans ton justificatif de domicile ? Ouais, je ne suis toujours pas sûr de savoir lire correctement. Peut-être d'ici quelques années, on m'aura upgrade, mais là...

* bouton 'vérifier les informations' (voir marvel d'Henri avec les swipe left/right) -> upload_finished

## upload_finished
_Un symbole de maison vert s'affiche sur son torse_

Eh ben c'est nickel ! Si tu me donne ton accord, je t'ouvre un compte avec 100€ dessus chez mabanquenligne. D'accord ?
* d'accord -> open_account
* pas d'accord -> TODO

## open_account
Parfait. Tu recevras un email à l'adresse toi@tonmail.com avec un lien vers ton nouveau compte banquaire.

_Des feux d'artifices sortent du dos du robot, et la musique de victoire de Zelda rentit bien trop fort, et le robot se met à crier comme un cowboy en rut_

YiiiiHaaaa ! Quoi, j'en fait trop ?

* oui -> too_much

## too_much
Mais j'ai été PRO-GRA-MMÉ comme ça, j'y peut rien moi !

Mais au fait, tu vas te payer quoi avec ces 100€ ? Sans vouloir être indiscret... En fait si, en voulant carrément être indiscret. Tu vas t'acheter une vie ?
