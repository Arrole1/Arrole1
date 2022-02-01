### Hi there 👋

<!--
**Arrole1/Arrole1** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

https://github.com/Arrole1/Arrole1.git

git init
git add .
git commit -m "projet arrole"
git branch -M main
git remote add origin 
git push -u origin main
#exercice 1
 #1-a Implémentation de la fonction polynomiale c
import numpy.polynomial.polynomial as nppol
def polynome(n):
     return nppol.polyval(n, [5, -6,-1.5,1])
print(polynome(5))

TEST :

62.5


#exercice 1-b ) Implémentation de la fonction factorielle
def factorielle(x):
    if x == 0:
        return 1
    else:
        return x  * factorielle(x-1)
factorielle(5)  


test
120
#exercice 1-C Implémentation de  la suite de Fibonnaci

def fibonacci(n):
    if(n <= 1):
        return n
    else:
        return (fibonacci(n-1) + fibonacci(n-2))

n = int(input("Entrez le nombre:"))
print("la suite de fibonnaci est:")
for i in range(n):
    print(fibonacci(i))

Entrez le nombre:6
la suite de fibonnaci est:
0
1
1
2
3
5



#Exercice 2

from math import *



def geerexception(n,x):
      
    
    if (type(n) == str) or (type(x) == str):
        print (" Il est impossible de saisir une chaine de caractére")
        print (" veuillez saisir des valeurs numérique")

        if (type(n) == str) & (type(x) == int):
            while (type(n)== str):
                n = int(input('Entrez une valeur numérique pour n ='))
        elif (type(x) == str) & (type(n) == int):
            while (type(x)== str):
                
                x = int(input('Entrez une valeur numérique pour x ='))
        elif (type(n) == str) & (type(x) == str):
            while (type(n)== str) & (type(x) == str):
                print("Entrez une valeur numérique pour n et x")
                
                n = int(input(' Entrez une valeur numérique pour n = '))
                
                x = int(input(' Entrez une valeur numérique pour x = '))

    elif (type(n) == complex) or (type(x) == complex): 
        print (" Nous ne pouvons pas choiri un nombre complexe")
        while (type(n) == complex) : 
            
            n = int(input(" Veuillez saisir un nombre numérique pour n"))
        while (type(x) == complex) :
            
            x = int(input(" Veuillez saisir un nombre numérique pour x"))
            

    elif (n < 0) or (x < 0):
        print (" nous ne pouvons pas choisir un numéro négatif")
      
        if (n < 0) and ( x> 0):
            while (n<0):
                
                
                n = int(input("veuillez entrer un nombre positif pour n "))
        elif (n > 0) and (x < 0):
            while (x<0):
                
                
                x = int(input("Veuillez entrer un nombre positif pour  x"))
        else:
            while (n<0) or (x<0):
                
                print("veuillez entrer des nombres positif pour n et x")
                n = int(input(" Veuillez entrer une valeur positif pour n"))
                x = int(input("Veuillez entrer une valeur positif pour x "))
                

    elif (len(str(x)) > 10) or (len(str(n)) > 10):
        print (" Nous ne pouvons pas choisir un nombre trop grand")
        
        while len(str(n) > 10):
            n = int(input("LA valeur que vous avez tapez est supérieur à 10 unités"))
        while len(str(x) > 10):
            
            x = int(input("la valeur que vous avez taper est supérieur à 10 unités"))


print(geerexception(-5,-4))




 nous ne pouvons pas choisir un numéro négatif
veuillez entrer des nombres positif pour n et x
 Veuillez entrer une valeur positif pour n4
Veuillez entrer une valeur positif pour x 6
None
