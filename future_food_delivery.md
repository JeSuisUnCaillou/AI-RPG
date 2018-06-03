# Large scale food delivery from the future
* begin : you are hungry at home
* end : you pay for your food delivery and eat
* failure : you don't eat and sleep hungry

## 1) intro
_Year 2050, It's the evening, you are home and hungry. The doorbell rings._

Ring Ring !
* open the door -> 2)
* ignore the bell -> 1)
* Insults -> 1)

## 2) greetings
_You see a delivery robot with one green eye, handing you a warm box labelled 'Amazon Food Prime' ou 'Foodex'_

Good evening citizen, here is your warm meal for tonight. It's spaghetti bolognaise.
* Thank you -> 5)
* I don't like this, I want something else -> 3)
* Nothing, i'm good. Not hungry. -> 8)
* Slam the door -> 9)
* Throw something at the robot -> 12)
* Insults -> 13)

## 3) changed_my_mind
_When you look around, you see a fleet of similar robots delivering boxes to your neighbors_

What would you like to eat instead ?
* I'd rather have tandoori chicken -> 4)
* Nothing, i'm good. Not hungry. -> 8)
* Slam the door -> 9)
* Throw something at the robot -> 12)
* Insults -> 13)

## 4) new_meal_proposal
_Your robot flies away while another robot of the fleet instantaneously brings you what you want_

Tandoori chicken for you. Are you satisfied with your new meal ?
* Yes, thank you -> 5)
* Not yet, i'd rather have paella -> 4)
* Nothing, i'm good. Not hungry. -> 8)
* Slam the door -> 9)
* Throw something at the robot -> 12)
* Insults -> 13)

## 5) payment_request
_Once you took your food, the robot's green eye becomes orange_

It costs 8,55€. How would you like to pay for our service, citizen ? We accept DNA, Voice recognition, QR code, cards, and cash.
* Give your DNA -> 6)
* Pay by QR Code -> 6)
* Pay by card -> 6)
* Give the cash -> 7)
* Nothing, i'm good. Not hungry. -> 8)
* Slam the door -> 9)
* Throw something at the robot -> 12)
* Insults -> 13)

## 6) payment_confirmed
- _You put your finger on a soft pad, and feel a tiny pinch. The robot's eye turns back to green_
- _You scan the robot's QR, verify the price, and send the payment. The robot's eye turns back to green_
- _You enter your card in the robot's card slot. You type your pin and take back your card. The robot's eye turns back to green_

You account as been debited of 8.55€. Thank you for choosing Amazon Food Prime.
* Take the food, Ok thanks bye ! -> 11)
* Slam the door -> 14)
* Throw something at the robot -> 12)
* Insults -> 13)

## 7) give_change
_You search in your wallet for the money, and give a 10€ bill to the robot. You heare coins falling inside the robot_

Please take your change, 1.45€

_The robot opens a little drawer_
* Take the change, Ok thanks bye ! -> 11)
* Slam the door -> 10)
* Throw something at the robot -> 12)
* Insults -> 13)

## 8) order_canceled
_The robot seems to be... thinking. It's eye quickly flips its color for a few seconds, then stops on green_

Understood, order canceled. Have a nice evening citizen.

_It flies away, joining a small fleet of similar robots delivering food to your neighbors_

* Close the door, and go on with my life -> GAME OVER
* Throw something at the robot -> 12)
* Insults -> 13)

## 9) order_canceled_through_door
_After few seconds, you hear the robotic voice through the door_

Understood, order canceled. Have a nice evening citizen.

_You spent the night hungry this time_

GAME OVER

## 10) forgot_change_through_door

_After few seconds, you hear the robotic voice through the door_

You forgot your change citizen.

_The bell rings_
* -> 7) without first text

## 11) eat_and_win
_You take your food, and the robot flies away, joining a small fleet of similar robots delivering food to your neighbors_

_You spend a lovely evening eating your tandoori chicken, mmmmh, life is good._

YOU WIN

## 12) throw_and_loose
_You throw [your shoe / your meal] at the robot. It just *bonks* on it_

Pleae don't deteriorate Amazon Food Prime's robots. Your order is canceled.

_The robot flies away, joining a small fleet of similar robots delivering food to your neighbors_

GAME OVER

## 13) stay_polite

_The robot shakes, it seems to be... laughing_

Please stay polite or I won't be able to understand what you say
* -> return

## 14) forgot_food_through_door
_After few seconds, you hear the robotic voice through the door_

You forgot your food citizen !
* ignore -> 14)
* open the door -> 11)

