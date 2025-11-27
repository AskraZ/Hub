gli esercizi ed i progetti si trovano su

[https://github.com/AskraZ/APPUNTI-UNICT-INF](https://github.com/AskraZ/APPUNTI-UNICT-INF)

## **WHILE**

il comando while genera un ciclo che finisce quando la sua condizione (o le sue condizioni) sono soddisfatte.

```c
// programma che prende due variabili e ne aumenta una finché non sarà uguale
// all'altra variabile
int main(){
int a = 3;
int b = 0;
while (a>3){
++b;
printf("b è aumentato di uno");
}
return 0;
}
```

si possono inserire anche due condizioni dentro un ciclo while:

```c

int main(){
int a = 5;
int b = 0;
int c = 2;
while (a>b || a>c){ // a>b "O" a>c, se avessimo voluto entrambe soddisfatte "&&"
++b;
++c;
} // il ciclo uscirà dall'esecuzione quando c=5 e b=3

}
```

## FOR

il ciclo for può essere definito come un ciclo definito, infatti a differenza del ciclo while sappiamo quando finirà.

```c
int main(){
int eta;
int maggiorenne = 18;

for (eta=0; eta<maggiorenne; ++eta){
printf("%s%d%s","il ragazzo ha" eta "anni");
}

}
```

## IF

con if definiamo una condizione per cui qualcosa può avvenire:

```c
int main(){
int eta = 18;
int etarichiesta = 18;

if (eta>=etarichiesta){
	printf("puoi entrare");
	}
else{

printf("non hai la giusta età per entrare");
}
}
```

### IF annidato

```c
int main(){
int eta = 18;
int etarichiesta = 18;
int prezzoentrata = 5;
int portafoglio = 2;

if (eta>=eta richiesta){
	printf("sei maggiorenne, potresti entrare");
	if (prezzoentrata>portafoglio){
	printf("mi dispiace, non hai abbastanza soldi");
	}
	else {
	printf("puoi entrare")
	portafoglio += -5;
	}
}
else{
printf("devi crescere un po'");
}
return 0;
}
```

## SWITCH

lo switch ti da la possibilità di configurare delle azioni in base ai “CASI”:

```c
int main(){

int input = 0;
printf("inserisci un numero da 1 a 3: ");
scanf("%d", &input);

switch (input){
case 1:
puts("hai inserito 1");
break;
case 2:
puts("hai inserito 2");
break;
case 3:
puts("hai inserito 3");
break;
}
return 0;
}
```

**non si possono usare i char nello switch**

## FUNZIONI

una funziona può essere definita all’esterno del main per migliorare la leggibilità e la riproducibilità del software:

```c
int square();
int main(){

int numero;
printf("inserisci il numero da elevare al quadrato: ")
scanf("%d", &numero);
int numeroalquadrato= square();
printf("%s%d", "il tuo numero al quadrato è: ", numeroalquadrato);
return 0;
}

int square(){

numeroalquadrato = numero * numero;
return numeroalquadrato;
}
```

le variabili definite all’interno di una funzione sono disponibili solo all’interno di essa.

# Array
un array è un gruppo di elementi immagazzinati in modo contiguo nella memoria.

![array-data-structure.webp](attachment:6095512e-6881-4db7-8795-1f626a0fcbef:array-data-structure.webp)

per fare riferimento ad una posizione, indichiamo il nome dell’array con l’indice contenuto tra parentesi quadre:

```c
int array[]={1,2,3,4,5};

array[2]= 4; // cambiamo l'elemento di indice 2 con il valore 4
```

un array di tipo char può memorizzare una stringa di caratteri.

## Array bi-dimensionali

a[i][j] → elemento di riga i e di colonna j

```c
a[2][2]={1,2}{3,4} 
```

$\begin{vmatrix}1 & 2 \\ 3 & 4\end{vmatrix}$

---
# Puntatori
i puntatori sono delle variabili.

un puntatore contiene un indirizzo di memoria.

```c
int a = 3;
&a // indirizzo memoria di a
int *ptr; // allocazione di memoria per ptr
ptr = null; //definiamo che il puntatore non punta a nulla
ptr = a;
stampa *ptr = 3;
stampa ptr = indirizzo di memoria di a;

```

## Const