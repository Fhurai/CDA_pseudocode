Variables chaine1, chaine2, commun en Chaïne
Variables i, j en Entiers
Début

    // Demande chaine1
    Ecrire "Veuillez saisir le premier mot :"
    Lire chaine1

    // Demande chaine2
    Ecrire "Veuillez saisir le deuxieme mot : "
    Lire chaine2

    // Initialisation des variables nécessaires
    i <- 0
    j <- 0
    commun = ""

    // Récupération de tout ce qui est commun.
    Tantque chaine1[i] <> "" faire
        Tantque chaine2[j] <> "" faire
            Si (chaine1[i] = chaine2[j]) alors
                Si (chaine[i-1] = chaine2[j-1]) alors
                    commun <- commun + chaine2[j]
                Finsi
            Finsi
        Fintantque
    Fintantque

    // Affichage de la sous-chaîne commune si elle existe sinon message d'erreur
    Si commun <> ""
        Ecrire "Les deux mots ont une partie commune : ", commun
    Sinon
        Ecrire "Erreur : aucune partie commune entre ces deux mots !"
    Finsi
Fin