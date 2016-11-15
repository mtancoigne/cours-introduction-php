[Accueil](README.md) | [Installation](00-installation.md) |  [Syntaxe](01-syntaxe.md) | [Variables](02-variables.md) | [Constantes](03-constantes.md) | **Opérateurs** | [Conditions](05-conditions.md) | [Boucles](06-boucles.md) | [Tableaux](tableaux.md) | [Fonctions](fonctions.md) | [Super-globales](super-globales.md) | [Classes / objets](classes-objets.md) | [Espaces de noms](espaces-de-noms.md)

# Opérateurs

Les opérateurs permettent de réaliser des opérations simples :

  - `+` Addition
  - `-` Soustraction
  - `*` Multplication
  - `/` Division
  - `%` Modulo
  - `.` Concaténation


```php
<?php
echo 3 + 3; // Affichera 6
echo 3 - 3; // Affichera 0
echo 3 * 3; // Affichera 9
echo 3 / 3; // Affichera 1
echo 3 % 3; // Affichera 0
echo 3 . 3; // affichera 33
echo 3.3; // Affichera 3.3 (nombre flottant)
```
Il est possible de réaliser ces opérations avec des variables :

```php
<?php
$valeur1 = 9;
$valeur2 = 3;

echo $valeur1 + $valeur2;
echo $valeur1 - $valeur2;
// etc...

$nouvelleVariable = $valeur1 * 7;
echo $nouvelleVariable; // Affichera 63
```
Il est aussi possible de modifier une variable directement :

```php
<?php
$maVar = 3;

$maVar = $maVar + 1;
// Equivaut à
$maVar += 4;

// Et celà fonctionne avec tous les opérateurs :

$maVar += 3;
echo $maVar // Affichera 6
$maVar -= 3;
echo $maVar // Affichera 0
$maVar *= 3;
echo $maVar // Affichera 9
$maVar /= 3;
echo $maVar // Affichera 1
$maVar %= 3;
echo $maVar // Affichera 0
$maVar .= 3;
echo $maVar // affichera 33
```

Il existe aussi des opérateurs spéciaux: `++` et `--`:

```php
<?php
$i=0;

$i++; // Ajoute 1
echo $i; // Affichera 1

$i--; // Enlève 1
echo $i; // Affichera 0

// Spécificités d'utilisation :
echo $i++; // Affiche 0. L'incrémentation se fait après l'affichage
echo $i; // Affiche 1

echo ++$i; // Affiche 2. L'incrémentation se fait avant l'affichage
echo $i; // Affiche 2
```
