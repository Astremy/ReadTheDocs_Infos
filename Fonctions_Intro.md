Une fonction est un bout de code que l'on peut appeler à de multiples reprises dans le programme. Cela suit le principe de "don't repeat yourself", ou "ne vous répétez pas".

Elle se défini ainsi :
```py
# définition
def nom_fonction(arguments):
  # code que l'on va faire
  ...
```

Souvent, on ne préférera pas mettre de print dans une fonction, sauf dans des cas spécifiques, car les interactions avec l'extèrieur doivent être controlés, et c'est plus propre (après ça dépend des cas)

Les fonctions ont des entrées que l'on appelle les arguments. A la définition de la fonction, on les met dans les parenthèses. ensuite, il faudra les spécifier a l'appel de la fonction.

Dans la fonction, on peut utiliser les variables que l'on as passé en paramêtres (et d'autres, mais il est mieux de se suffire de ceux passés en params).

Pour que la fonction renvoie des informations utilisables, il faut utiliser le mot-clé return. On récupèrera ensuite la sortie a l'appel de la fonction

Exemple :
```py
# On crée une fonction add, quiprend deux paramêtres
def add(a,b):
  # Renvoi l'addition des deux nombres passés en paramêtres
  return a+b

# On utilise la fonction add
var1 = add(4,8)
var2 = add(5,0)
print(add(var1,var2))
```

Exerices :

```md
## Premier Exo
Faire une fonction qui calcule les n premiers nombres impairs.

## Second Exo
Faire une fonction qui va calculer les solutions d'une équation du second degré avec a, b et c donné (forme : ax² + bx + c = 0)
```
