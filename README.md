# Tema 2 AA - Pocris Sabin 322CB

## TL;DR

Pentru aceasta tema, am ales sa sa adaug variabilele reducerii SAT intr-un
hashmap, mai concret intr-un dictionar, intrucat am realizat tema in Python).

Oricare variabila $x_{ij}$, cu semnificatia ca al $i$-lea nod din clica este nodul $v$,
are asociat in hasmap un string de forma `"i,j"`.

Graful este reprezentat de o matrice de adiacenta.


## Descrierea programului
 
In primul rand, am ales sa citesc din fisier si sa construiesc matricea de adiacenta, ce
reprezinta graful. Urmatorul pas a fost sa construiesc hashmap-ul ce asociaza fiecarei 
variabile din SAT un string de forma `"i,j"`.

Am construit 3 bucle, una pentru fiecare conditie din
enuntul reducerii, pentru a construii clauzele necesare:
1. există un al $i$-elea nod în clica
2. toate elementele clicii sunt unice
3. oricare doua noduri din clica să aibă muchie între ele

In final, adaug datele necesare formatului `DIMACS` si scriu clauzele generate mai sus in
fisierul de output.