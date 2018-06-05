# Le Sphynx moderne
* begin: tu marches dans la rue et rencontre un type étrange qui te propose des énigmes contre de l'argent
* end: tu as déjoué ses intrigues et il te donne de l'argent IRL !
* fail: tu n'as pas déjoué ses intrigues et il te donne envie de rejouer pour la revanche

 -> enchaîne sur _l'étrange personnage change de casquette, ainsi que de ton. Il entame les démarches pour te faire ouvrir un compte dans sa banque afin de te donner l'argent que tu as gagné_ -> scénario d'onboarding

 -> technical need : certaines steps doivent avoir un 'compteur' qui permet de choisir le n-ième message en fonction du nombre de fois que l'utilisateur y passe (good_answer, bad_answer, no_answer, insults, etc..)

## intro
_Tu marches dans la rue, pas loin de chez toi, et croises un type avec un énorme chapeau. Assez étrange_

Eh toi ! Ouais toi, pourquoi tu vois d'autres clanpins au bout de ton téléphone là ? Tu veux pas jouer à un jeu d'énigmes avec moi ?

_L'homme déploie un sourire digne des pire creepy pasta_

* Oui, pourquoi pas -> game_accepted
* Non, dégage -> game_not_accepted

## game_accepted
Excellent Smitters ! Viens on marche un peu.

Je me présente, moi c'est Sept, et on voici ta première énigme.

-> Question 1

## bad_answer
_La musique de la boule noire de Motus résonne atour de vous, comme provenant de nulle part et partout à la fois._

_Quant à l'homme, il a désormais la voix de Julien Lepers._

C'est non.

## good_answer
_la musique de découverte d'un objet dans Zelda retentit_

Oooow yeaaah baby !

-> Question suivante

## dunno
**(Au choix)**

Boah allez ! Fait un effort, propose au moins un truc t'as vu !

Franchement c'est pas si dur, t'exagères.

Tu peux le faire, je crois en toi !

## game_not_accepted
_L'homme a l'air sincèrement triste de ta réponse. Il réajuste son chapeau sur le côté - en mode coquin pense-t-il, mais ça le rend juste encore plus étrange._

Boaaaah alleeeez ! Si tu gagnes, je t'offre 100€ IRL. Juré craché !

_L'homme tente de cracher par terre, mais se rate. Il essuie piteusement sa lèvre, conscient d'avoir raté son effet_

* lol le bolosse quoi
* bon ok, tu me fait pitié -> game_accepted
* non toujours pas -> the_end

## question_1
_Il se retient visiblement de sourire en se bouffant la lèvre_

Quel est la différence... entre un pigeon ?
* Aucune. Les deux pattes ont la même taille, surtout la gauche. -> good_answer
* Il ne sait ni voler. -> good_answer
* je ne sais pas -> dunno
* [mauvaise réponse] -> bad_answer

## question_2
_A force de discuter avec lui, tu n'as pas fait attention aux alentours. Mais tu remarques maintenant que tu es en Asie_
* TODO

## question_3
_Les alentours ont encore mystérieusement changé. Tu as l'impression d'être dans un bazar algérien_
* TODO

## question_4
_Cette fois tu as bien fait attention, mais rien n'y fait. Tu t'es encore fait surprendre par le changement de décor_
* TODO


## why_changing_decor
TODO (il y a des indices dans les décors, genre coluche en indice de la question 1)

## you_win
_L'homme, déconfit, claque des doigts. Tu reconnais une rue près de chez toi_

Tu es bien trop fort pour mes énigmes bas de plafond. Allez, tu mérites bien tes 100€.

_L'homme retire son grand chapeau, il est désormais en costume propre_

A une condition : Tu dois ouvrir un compte dans... _il cherche rapidement autour de lui_ ...cette banque !

* OK -> you_win_2
* Nope -> TODO

## you win_2
_L'homme entre dans l'agence banquaire, ouvre un bureau, s'assoie dans le fauteuil du conseiller et te présente le siège dans lequel s'assoient habituellement les clients_

Assieds-toi, on va régler les formalités ensemble. 

## you_loose
_Tout excité par sa victoire, l'homme saute sur place comme un enfant qui aurait bouffé trop de sucres_

Peeer-duuu perdu-perdu-perdu ! HAHA ! Qu'est-ce que tu dis de ça hein ? Avoue que t'as la rage. Avouuuue !

_Se calmant brusquement, il se penche à ton oreille et murmure_

Tu voudrais pas remonter dans le temps, pour une revanche, mmmh ? Il suffirait de demander tu sais...

* remonter dans le temps / recommencer -> intro
* non merci, allez salut -> THE END

## the_end
_Déçu, l'homme s'en va... en marchant à reculons et en maintenant le contact visuel. Creepy._
 THE END

