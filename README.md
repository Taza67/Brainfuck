# Brainfuck

## Créateur(s)

- **Nom(s) :** AKIL
- **Prénom(s) :** Mourtaza
- **Projet :** Interpréteur-Compilateur pour le langage *Brainfuck*

## Programmes

### Liste des programmes

- **brainfuck**

### Descriptif des programmes

- **brainfuck :**
  - Le programme `interprète` un programme écrit en langage *Brainfuck*.
  - Le programme `compile` un programme écrit en langage *Brainfuck* en :
    - ***Bytecode*** adapté à la machine virtuelle intégrée au programme.
    - ***C***
    - ***Python***
  - Le programme `compile` du bytecode obtenu à partir du programme *brainfuck*
	lui-même en :
    - ***C***
    - ***Python***
  - Le programme `décompile` du bytecode obtenu à partir du programme
  	*brainfuck* lui-même en
	***Brainfuck***.

## Commandes du Makefile

Pour compiler le programme **Brainfuck**, il faut taper la commande `make`
depuis la *racine du projet*.

- `make help`    : affiche une notice d'utilisation du Makefile.
- `make clean`	 : supprime tous les fichiers objets, tous les fichiers
				   résiduels et tous les exécutables.
- `make build` 	 : compiler le programme **brainfuck**.
- `make rebuild` : recompiler le programme **brainfuck**.

## Exécution des programmes

Les exécutables, après leur compilation, sont situés à *racine du projet*.

### Programme **brainfuck**

Depuis la racine, l'appel se ferai ainsi :

    ./brainfuck [<option> [<sous-option>]] [<entree>] [<sortie>]

Sans aucun argument, la notice d'utilisation sera affichée par défaut.

#### Notice d'utilisation

Voici un aperçu de la notice d'utilisation du programme :

    - Interpréteur du langage Brainfuck
    - Usage: brainfuck [<option> [<sous-option>]] [<entree>] [<sortie>]

      -    [<option>]                   :    -h    affiche la notice d'utilisation
                                             -c    compile le programme en entrée
                                             -cb   compile le bytecode en entrée
                                             -i    interprète le programme en entrée
                                             -ib   exécute le Bytecode en entrée
                                             -d    décompile le bytecode en entrée

      +    -    [<sous-option>]         :    python    compile en Python
                                             c         compile en C
                                             + optionnel pour l'option {-c}
                                             + nécessaire pour l'option {-cb}
                                             bytecode  compile en C
                                             + optionnel pour l'option {-c}

      -    [<entree>]                   :    code source en langage Brainfuck
                                             + nécessaire pour l'option {-c}
                                             + nécessaire pour l'option {-i}
                                             bytecode
                                             + nécessaire pour l'option {-cb}
                                             + nécessaire pour l'option {-ib}
                                             + nécessaire pour l'option {-d}

      -    [<sortie>]                   :    nom du fichier de sortie
                                             + nécessaire pour l'option {-c}
                                             + nécessaire pour l'option {-cb}
                                             + nécessaire pour l'option {-d}

      -    default                      :    affiche la notice d'utilisation
