# Faire une demande d'aide

Quand on fait une demande d'aide, il ne faut pas la bacler, plus elle sera complete, plus facilement/efficacement l'on pourra vous aider.

## A ne jamais faire

- Faire une photo de son écran avec son téléphone

En premier temps, envoyez ce qui est demandé plus bas. Il se peut que l'on vous demande d'envoyer une **capture d'écran** de votre code.
Jamais, ou presque, l'on ne vous demandera une photo.

- Envoyer des fichiers/une archive zip

Si vous devez envoyer des fichiers, donnez un lien contenant votre fichier.
Cela peut être fait via un [github](https://github.com/) ou un [gist](https://gist.github.com/) si vous avez plusieurs fichiers,
ou, si vous en avez un seul ou ne souhaitez pas vous inscrire/connecter a github,
il y a [hastebin](https://hastebin.com/) ou [artemix](https://paste.artemix.org/)

- Manquer de respect à ceux qui aident

Ceux qui regardent votre code et cherchent a vous aider le font naturellement, ils n'en ont aucune obligation.
Ainsi, si vous vous montrez irrespetueux envers ces derniers, cela fera juste vous ralentir pour trouver la solution/progresser.
Si *eux*, vous manquent de respect, rapprochez vous d'un modérateur qui se chargera de régler le problème,
n'essayez pas de rentrer dans leur jeu, ou c'est vous qui risquez d'être sanctionné.
Mais dites vous que 90 % du temps, c'est les aidés qui posent probleme, et non les aideurs.

- Attendre que l'on vous donne le code de solution tout fait

C'est un serveur d'entraide, le but n'est pas de transformer les gens en assistés,
nécessitant forcément de revenir demander de l'aide a chaque bug.
Nous cherchons a vous inciter a chercher les erreurs par vous-même en vous guidant sur le bon chemin.

Ainsi, ne commencez pas a vous plaindre que l'on ne vous donne pas la solution, mais plutot des indices et que l'on vous laisse trouver.

## Avant de poster un message de demande d'aide

Avant de poster un message de demande d'aide, il y a certaines questions a se poser.

#### Quel probleme ait-je ?
Est-ce une fonction qui ne marche pas ? Une mauvaise variable ?
Est-ce que le problème fait une erreur dans la console, ou cela ne marche simplement pas ?
Prenez le temps de vous demander quelle partie du programme ne marche pas, et de débugguer, pour voir **ou** cela coince.
Cela aide souvent beaucoup à régler le problème.

#### Est-ce que j'ai bien cherché sur google ?
Est-ce que vous avez cherché sur google votre probleme ? Pas en toutes lettres, mais en mots-clés ? En anglais ?
Avez-vous bien vérifié les premier liens Stack Overfow (Si vous n'avez pas de lien Stack overflow, vous n'avez pas bien fait votre recherche)?

Souvent, chercher l'erreur de la console si on en as une permet de bien aider.

## Comment faire un message de demande d'aide ?
*les messages montrés sont des exemples*

Ne demandez pas si quelqu'un s'y connais en un domaine en particulier, ou si l'on peut vous aider, cela ne fera que ralentir de devoir.

Commencez par une formule de politesse :
```
Bonjour/Bonsoir,
```

Posez le contexte, en effet, ceux qui vous aident ne savent pas ce que vous faites,
et ne peuvent pas magiquement deviner (enfin si, mais il vaut mieux expliquer):
```
Je fait un programme tkinter, ou je tente de faire un rpg textuel, ou l'on écrit les actions que l'on veut faire.
Seulement, je suis face a un probleme concernant les combats.
```

Après avoir fait la présentation globale de votre probleme, dites clairement ce qui ne va pas.
Pour cela, deux possibilités :

### Cela renvoie une erreur :
Dites que vous avez une erreur, donnez le message d'erreur, la ligne de la fonction qui pose probleme

```
Dans la fonction de combat (l 15-23), cela me fait une erreur KeyError: 'arme'.
Je défini le dictionnaire qui pose l'erreur en ligne 13, et la boucle juste après est sensée ajouter la clé arme.
```

### Cela ne renvoie pas d'erreur :
Dire ce que c'est sensé faire, ce que cela fait/ne fait pas. Ce qui se passe exactement.. Donnez le maximum de pistes possibles

```
Ma fonction de combat (l 15-23) fait combattre le joueur et l'animal, en faisant une action par seconde,
jusqu'à ce qu'il y en ait un qui perde.
Seulement, quand la fonction se lance, la fenetre tkinter se freeze pendant une dizaine de secondes (le temps du combat je pense),
ne répond plus, et re-répond quand le combat est fini, tandis que toutes les actions sont mises d'un coup dans l'affichage tkinter.
```

Faites une phrase de politesse pour clore votre question

```
Si vous avez des pistes pour résoudre le problème, merci d'avance.
```

Enfin, envoyez les fichiers de votre programme pour que l'on puisse chercher ce qui ne va pas.

Si vous avez une erreur, mettez aussi la Traceback entière, et pas que l'erreur.

```
Fichiers :
main.py : https://hastebin.com/lurakuqiti.py
data.py : https://hastebin.com/ehekihezub.py

Traceback : https://hastebin.com/osabuhunir.sql
```

### A quoi sert une traceback

La traceback indique tout le fonctionnement du programme, les erreurs, d'ou cela viens, la ligne, le fichier.

Ainsi, c'est une mine d'or pour le programmeur. Et ceux qui aident savent les lire

Il faut envoyer la traceback complete a part, car si quelqu'un qui aide a besoin de voir plus que la simple erreur
(dite plus haut dans la question) pour pouvoir aider, ou que l'erreur n'est pas indicative du probleme, la traceback aide beaucoup.

Voici un exemple de Traceback :
```
C:\Users\Astremy\Desktop\astremy.com\Piscord\PyPI\piscord\Piscord.py:120: RuntimeWarning: coroutine 'ClientResponse.json' was never awaited
  response = await self.api_call("/gateway")
RuntimeWarning: Enable tracemalloc to get the object allocation traceback
Traceback (most recent call last):
  File "C:\Users\Astremy\Desktop\astremy.com\Piscord\PyPI\test.py", line 112, in <module>
    bot.run()
  File "C:\Users\Astremy\Desktop\astremy.com\Piscord\PyPI\piscord\Piscord.py", line 161, in run
    self.loop.run_until_complete(self.begin())
  File "C:\Users\Astremy\AppData\Local\Programs\Python\Python38\lib\asyncio\base_events.py", line 612, in run_until_complete
    return future.result()
  File "C:\Users\Astremy\Desktop\astremy.com\Piscord\PyPI\piscord\Piscord.py", line 121, in begin
    await self.__main(response["url"])
TypeError: 'NoneType' object is not subscriptable
Exception ignored in: <function _ProactorBasePipeTransport.__del__ at 0x0000022FFB34E0D0>
Traceback (most recent call last):
  File "C:\Users\Astremy\AppData\Local\Programs\Python\Python38\lib\asyncio\proactor_events.py", line 116, in __del__
  File "C:\Users\Astremy\AppData\Local\Programs\Python\Python38\lib\asyncio\proactor_events.py", line 108, in close
  File "C:\Users\Astremy\AppData\Local\Programs\Python\Python38\lib\asyncio\base_events.py", line 715, in call_soon
  File "C:\Users\Astremy\AppData\Local\Programs\Python\Python38\lib\asyncio\base_events.py", line 508, in _check_closed
RuntimeError: Event loop is closed
```

Le réel probleme est a la première ligne, une coroutine non awaited. C'est un bug plutot courant et très facile a résoudre.

Seulement, l'erreur en soit est un Runtime Error, donc si vous donnez juste l'error, cela n'aidera pas.
Ainsi, dans ce cas la, la traceback se retrouve très utile, et permet d'identifier le probleme, la ligne, et le fichier.

Bonne chance pour faire des questions propres à l'avenir !
