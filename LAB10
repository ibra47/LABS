#Classes et objets

#ex1
class Voiture:
    def __init__(self, marque='Ford', couleur='rouge'):
        self.marque = marque
        self.couleur = couleur
        self.pilote = 'personne'
        self.vitesse = 0

    def choix_conducteur(self, nom):
        self.pilote = nom

    # ex1.2
    def accelerer(self, taux, duree):
        if self.pilote == 'personne':
            return

        #variation de la vitesse
        varvit = taux * duree
        self.vitesse += varvit

    #faire apparaitre les proprietes presentes de la voiture (matque, couleur etc.)
    def affiche_tout(self):
        print(self.marque, self.couleur, "pilotée par",self.pilote, ",","vitesse= ",self.vitesse,"m/s.")

    # méthodes __repr__ et __eq__
    def __repr__(self):
        return f'Voiture({self.marque}, {self.couleur}, {self.pilote}, {self.vitesse})'
    def __eq__(self, other):
        return (self.marque == other.marque and
                self.couleur == other.couleur and
                self.pilote == other.pilote and
                self.vitesse == other.vitesse)

#Affichage des attributs
a1 = Voiture('Peugot', 'Bleue')
a2 = Voiture(couleur='verte')
a3= Voiture('Mercedes')
a1.choix_conducteur('Roméo')
a2.choix_conducteur('Juliette')
a2.accelerer(1.8, 12)
a3.accelerer(1.9, 11)

a2.affiche_tout()
a3.affiche_tout()

#ex 2


class CompteBancaire:
    def __init__(self, nom='Dupont', solde=1000):
        self.nom = nom
        self.solde = solde

    def depot(self,somme):
        self.solde  += somme
    def retrait(self,somme):
        self.solde -= somme

    #affichage de tout
    def affiche(self):
        print("Le solde du compte bancaire de",self.nom,"est de","$", self.solde,"CDN.")

# méthodes __repr__ et __eq__
    def __repr__(self):
        return f'CompteBancaile({self.nom}, {self.solde})'
    def __eq__(self, other):
        return (self.nom == other.nom and
                self.solde == other.solde)

#affichahe des attributs
#compte1
compte1=CompteBancaire('Duchmol',800)
compte1.depot(350)
compte1.retrait(200)
compte1.affiche()

#compte2
compte2 = CompteBancaire()
compte2.depot(25)
compte2.affiche()

#add monthly reiteration later!
class CompteEpargne(CompteBancaire):
    def __init__(self, taux=0.3//100):
        self.taux = taux

    def changeTaux(self,valeur):
        self.taux = valeur

    def capitalisation(nombreMois):
        for i in range(nombreMois):
            nombreMois+1


