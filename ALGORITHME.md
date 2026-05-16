EXERCICE_1
programme  remplissage_de_deux_methodes_differentes
const tmax = 5
type vecteur = tableau [1..tmax] entier 
var v : vecteur 
var i : entier
       // 1er methode
pour i <--1 à tmax faire 
ecrire("saisir 0")	
lire (v[i])
finpour
pour i <--1 à tmax faire 
ecrire(v[i]) 
finpour 
     //2em methode
ecrire("remplissage du tableau")	 
v[1]<-0
v[2]<-0
v[3]<-0
v[4]<-0
v[5]<-0
pour i <-- 1 à tmax faire 
ecrire (v[i])
finpour 
fin 

||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||
EXERCICE_2
programme  remplissage_de_voyelle
type vecteur = tableau [1..6] entier 
var v : vecteur 
var i : entier
debut    
ecrire("remplissage du tableau avec des voyelles") 
v[1]<--'a' 
v[2]<--'o' 
v[3]<--'u' 
v[4]<--'e' 
v[5]<--'i' 
v[6]<--'h'   
pour i <-- 1 à 6 faire 
ecrire(v[i])
finpour 
fin
 //le tableau peut etre de reel d'entier ou de caractere et ne pas oublier les carateres '' oubien chaine de caractere""
||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||
EXERCICE_3
programme  remplissage_de_notes
type vecteur = tableau [1..9] réel  
var v : vecteur 
var i : entier
debut     
pour i <-- 1 à N faire 
Ecrire("veullez saisir les notes :")
Lire(v[i])
finpour 
Ecrire("Affichage des notes")
pour i <-- 1 à N faire 
Ecrire(v[i])
finpour
fin

||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||
EXERCICE_4
programme  remplissage_de_notes_et_calcule_de_moyenne
const tmax = 100
type vecteur = tableau [1..tmax] réel  
var v : vecteur 
var N,i: entier
var moyenne,s : reel
debut
repeter 
   Ecrire("saisir la taille maximal du tableau")
   Lire (N)
jusqua'a (N> 0 et N <=tmax) 
    s<-- 0   
pour i <-- 1 à N faire 
  Ecrire("veuillez saisir la note  :",i)
  Lire(v[i])
  s<-- s + v[i]
finpour 
   Ecrire("Affichage des notes")
pour i <-- 1 à N faire 
   Ecrire(v[i])
finpour 
moyenne <-- s/N 
Ecrire("le moyenne est :",moyenne)  
fin

||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||
EXERCICE_5
programme note_superieur_a_la_moyenne
Const tmax = 100
Type vecteur = tableau [1..tmax] réel  
Var v : vecteur 
var N,i: entier
var moyenne,s,note : réel
Debut
Répeter 
   Ecrire("saisir la taille maximal du tableau")
   Lire (N)
Jusqua'a (N> 0 et N <=tmax) 
s<-- 0   
Pour i <-- 1 à N faire 
  Ecrire("veuillez saisir la note  :",i)
  Lire(v[i])
  s<-- s + v[i]
finpour 
   Ecrire("Affichage des notes :")
Pour i <-- 1 à N faire 
   Ecrire(v[i])
finpour 
   moyenne <-- s/N

Pour i <--1 a N faire
   Si(v[i] > moyenne) alors        
  Ecrire(v[i]) 
   finsi
finpour 
    
fin

||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||
EXERCICE_6
programme nombre_negative_et_positive
Const tmax = 100
Type vecteur = tableau [1..tmax] entier  
Var v : vecteur 
var N,i: entier

var compteur_negative,compteur_positive : entier

Debut
Répeter 
   Ecrire("saisir la taille maximale du tableau")
   Lire (N)
Jusqua'a (N> 0 et N <=tmax)    
Pour i <-- 1 à N faire 
  Ecrire("veuillez saisir l'element :",i)
  Lire(v[i]) 
finpour 
   Ecrire("Affichage des elements :")
Pour i <-- 1 à N faire 
   Ecrire(v[i])
finpour 
compteur_negative <--0
compteur_positive<--0
Pour i <--1 à N faire
      Si (v[i] > 0) alors        
      compteur_positive <-- compteur_positive + 1
	  finsi
	  Si (v[i] < 0) alors        
      compteur_negative <-- compteur_negative + 1
	  finsi
finpour
      Ecrire("le nombre de valeur positive est :",compteur_positive)
	  Ecrire("le nombre de valeur negative est : ",compteur_negative)   
fin

||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||
EXERCICE_7
programme produit_negative_somme_positive
Const tmax = 100
Type vecteur = tableau [1..tmax] entier  
Var v : vecteur 
var N,i: entier

var produit_negative,somme_positive: entier

Debut
Répeter 
   Ecrire("saisir la taille maximale du tableau")
   Lire (N)
Jusqu'a (N> 0 et N <=tmax)    
Pour i <-- 1 à N faire 
  Ecrire("veuillez saisir l'element :",i)
  Lire(v[i]) 
finpour 
   Ecrire("Affichage des elements :")
Pour i <-- 1 à N faire 
   Ecrire(v[i])
finpour 

produit_negative <--1
somme_positive<--0
Pour i <--1 à N faire
      Si (v[i] >= 0) alors        
	   somme_positive<--somme_positive + v[i]
	  finsi
	  Si (v[i] < 0) alors        
	   produit_negative <-- produit_negative * v[i]
	  finsi
finpour
      Ecrire("la somme des valeurs posititve est  :",somme_positive)
	  Ecrire("le produit des valeurs negatives est :",produit_negative)   
fin

||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||
EXERCICE_8
programme nombre_premier_nombre_parfait
Const tmax = 100
Type vecteur = tableau [1..tmax] entier  
Var v : vecteur 
var N,i: entier

var npr,npa,ndiv,smdiv,j,cpt: entier
 
 
Debut
Répeter 
   Ecrire("saisir la taille maximale du tableau")
   Lire (N)
Jusqu'a (N> 0 et N <=tmax)    
Pour i <-- 1 à N faire 
  Ecrire("veuillez saisir l'element :",i)
  Lire(v[i]) 
finpour 
   Ecrire("Affichage des elements :")
Pour i <-- 1 à N faire 
   Ecrire(v[i])
finpour 

npr<--0
npa<--0

Pour i <--1 à N faire
ndiv <-- 0
     Pour j <--1 à v[i] faire 
        Si (v[i] mod j = 0) alors        
		 ndiv <-- ndiv + 1
	   finsi
	 finpour
	    Si(ndiv = 2) alors 
	    npr<--npr + 1
		finsi
          
smdiv <--0
		 Pour j<--1 à v[i]/2 faire
	    Si (v[i] mod j=0) alors        
	   smdiv <--smdiv +j 
	  finsi
	  finpour
	  Si(smdiv = v[i]) alors
	  npa <-- npa +1
	  finsi
finpour
      Ecrire("le nombre de nombre premier est :",npr)
	  Ecrire("le nombre de nombre parfait est :",npa)   
fin


||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||
EXERCICE_9
programme recherche_de_une_valeur_dans_le_tableau
Const tmax = 100
Type vecteur = tableau [1..tmax] entier  
Var v : vecteur 
var N,i: entier

var x,cpt: entier
 
Debut
Répeter 
   Ecrire("saisir la taille maximale du tableau")
   Lire (N)
Jusqu'a (N> 0 et N <=tmax)    
Pour i <-- 1 à N faire 
  Ecrire("veuillez saisir l'element :",i)
  Lire(v[i]) 
finpour 
   Ecrire("Affichage des elements :")
Pour i <-- 1 à N faire 
   Ecrire(v[i])
finpour 

       Ecrire("saisir la valeur de x")
       Lire(x)
cpt<--0
Pour i<-- 1 à N faire 
    Si(v[i]= x) alors 
	cpt <-- cpt + 1
	finsi
finpour 
     Ecrire("le nombre de presence de x est",cpt, "fois")
fin 

||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||
EXERCICE_10
 programme recherche_de_une_valeur_puis_echange
Const tmax = 100
Type vecteur = tableau [1..tmax] entier  
Var v : vecteur 
var N,i: entier

var x,y: entier
 
Debut
Répeter 
   Ecrire("saisir la taille maximale du tableau")
   Lire (N)
Jusqu'a (N> 0 et N <=tmax)    
Pour i <-- 1 à N faire 
  Ecrire("veuillez saisir l'element :",i)
  Lire(v[i]) 
finpour 
   Ecrire("Affichage des elements :")
Pour i <-- 1 à N faire 
   Ecrire(v[i])
finpour 

       Ecrire("saisir la valeur de x et de y")
       Lire(x,y)
	   
Ecrire("Tableau AVANT modification : ")
   Pour i <-- 1 à N faire 
      Ecrire(v[i])
   finpour 

   Pour i <-- 1 à N faire
      Si (v[i] = x) alors
         v[i] <-- y
      finsi
   finpour

   Ecrire("Tableau APRES modification : ")
   Pour i <-- 1 à N faire 
      Ecrire(v[i])
   finpour 
fin

||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||
EXERCICE_11
programme addition_de_deux_tableaux
Const tmax = 100
Type tab = tableau [1..tmax] entier  
Var t1,t2,t3 : tab 
var N,i: entier

 
Debut
Répeter 
   Ecrire("saisir la taille maximale du tableau")
   Lire (N)
Jusqu'a (N> 0 et N <=tmax)
    
Pour i <-- 1 à N faire 
  Ecrire("veuillez saisir l'element :",i,"de t1")
  Lire(t1[i]) 
finpour 
Pour i <-- 1 à N faire 
  Ecrire("veuillez saisir l'element :",i,"de t2")
  Lire(t2[i]) 
finpour 
   
Pour i <-- 1 à N faire 
  t3[i]<--t1[i]+ t2[i]
finpour 
Pour i <-- 1 à N faire 
  Ecrire(t3[i]) 
finpour 
       
fin

||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||
EXERCICE_12
programme produit_scalaire
Const tmax = 100
Type tab = tableau [1..tmax] entier  
Var t1,t2 : tab 
var N1,N2,i,j,ps: entier

 
Debut
Répeter 
   Ecrire("saisir la taille maximale du tableau 1")
   Lire (N1)
Jusqu'a (N1> 0 et N1 <=tmax)
    
Pour i <-- 1 à N1 faire 
  Ecrire("veuillez saisir l'element :",i,"de t1")
  Lire(t1[i]) 
finpour 
Répeter 
   Ecrire("saisir la taille maximale du tableau 2")
   Lire (N2)
Jusqu'a (N2> 0 et N2 <=tmax)
Pour i <-- 1 à N2 faire 
  Ecrire("veuillez saisir l'element :",i,"de t2")
  Lire(t2[i]) 
finpour 
ps<--0 
Pour i <-- 1 à N1 faire 
Pour j <-- 1 à N2 faire 
ps<--  ps + t1[i]* t2[j]
finpour 
finpour
  Ecrire("le produit scalaire est : ",ps)        
fin

||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||
EXERCICE_13
programme valeur_maxiamal_et_position
Const tmax = 100
Type vecteur = tableau [1..tmax] entier  
Var v: vecteur 
var N,i,max,position: entier
Debut
Répeter 
   Ecrire("saisir la taille maximale du tableau")
   Lire (N)
Jusqu'a (N> 0 et N <=tmax)    
Pour i <-- 1 à N faire 
  Ecrire("veuillez saisir l'element :",i)
  Lire(v[i]) 
  finpour
   Ecrire("Affichage des elements :")
   
Pour i <-- 1 à N faire 
   Ecrire(v[i])
finpour
Pour i <-- 1 à N faire
      Si (i = 1) alors
         max <-- v[i]
		 position <--i
		  Sinon
          Si (v[i]>max)alors 
        max<--v[i]
        position<-- i		
             finsi
	 finsi
   finpour
     Ecrire("la valeur maximal est :",max,"et sa position est",position)
fin
||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||
EXERCICE_14
programme valeur_extremes
Const tmax = 100
Type vecteur = tableau [1..tmax] entier  
Var v: vecteur 
var N,i,max,min: entier
Debut
Répeter 
   Ecrire("saisir la taille maximale du tableau")
   Lire (N)
Jusqu'a (N> 0 et N <=tmax)    
Pour i <-- 1 à N faire 
  Ecrire("veuillez saisir l'element :",i)
  Lire(v[i]) 
  finpour
   Ecrire("Affichage des elements :")
   
Pour i <-- 1 à N faire 
   Ecrire(v[i])
finpour
Pour i <-- 1 à N faire
      Si (i = 1) alors
         max <-- v[i]
		min <-- v[i]
		  Sinon
             Si (v[i]>max)alors 
             max<--v[i]
		     finsi
		      Si (v[i]<min)alors 
       		   min<--v[i]
               finsi
	 finsi
   finpour
     Ecrire("la valeur extreme sont :",max,"et",min)
fin

||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||
EXERCICE_15
programme trie
Const tmax = 100
Type vecteur = tableau [1..tmax] entier  
Var v: vecteur 
var N,i,j,stock: entier
Debut
Répeter 
   Ecrire("saisir la taille maximale du tableau")
   Lire (N)
Jusqu'a (N> 0 et N <=tmax)    
Pour i <-- 1 à N faire 
  Ecrire("veuillez saisir l'element :",i)
  Lire(v[i]) 
  finpour
   Ecrire("Affichage des elements :")
   
Pour i <-- 1 à N faire 
   Ecrire(v[i])
finpour

Pour i <-- 1 à N-1 faire
Pour j <-- 1 à N-i faire
      Si (v[j]> v[j+1]) alors
	  stock <--v[j]
	  v[j]<--v[j+1]
	  v[j+1]<--stock
	  finsi
   finpour      
   finpour
   Ecrire("le tableau trie par ordre croissant est :")
 Pour i <-- 1 à N faire 
     Ecrire(v[i])
   finpour	 
fin

