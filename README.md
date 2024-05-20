# Edgemony CB10 - Exercises

## Venerdì 17/05
- Voca.js: https://vocajs.pages.dev/

### Esercizi

#### Trova il positivo:
dato un array di numeri [-1, -2, -10, 2, 5];

scriviamo due cicli for che soddisfano ognuno una condizione:
1. Stampare in console solo i numeri > 0
2. Deve interrompere al primo numero > 0 l'esecuzione del for (break)

----

#### Palindromi:
abbiamo visto come si trova una parola palindroma, ma non l'abbiamo fatto in modo efficente.
Quello che dovremo fare invece è: prendere una parola dall'utente tramite prompt, scomporla in array
ed usare un for per poter controllare se è palindroma.

nel caso in cui non troviamo corrispondenza usiamo dal for e stampiamo in console.log un messaggio.
se nell'ultimo carattere della parola non abbiamo riscontrato errori stampiamo un console.log con "Successo! è un palindromo!"


tips:
ogni carattere è uguale al suo elemento specchio nella parola
elemento ad indice 0 === elemento ad indice fine meno -1
elemento ad indice 1 === elemento ad indice fine meno -2
elemento ad indice i === elemento ad indice fine meno (i * -1) -1 /// length - i - 1 

```js
for(){

    if( elemento corrisponde a...){}

    isLast = index === length -1;

    if(elemento è l'ultimo dell'array...){

    }
}
```


## Giovedì 16/05
- Voca.js: https://vocajs.pages.dev/


### Esercizi

Rifacciamo l'esercizio del quiz di ieri in cui chiediamo all'utente di rispondere a domande a risposta multipla, in particolare però:
- Raccogliamo tutte le risposte date dall'utente anche dentro un array "risposte";
- Quando diamo il risultato finale, mostriamo anche tutte le risposte date dall'utente dentro un solo console.log e dentro mettiamo anche la lunghezza del nostro array

```js
const risposte = []; // salviamo tutte le risposte
let score = 0;
let risposta;

risposta = ...;
// aggiungere al nostro array di risposte;


....

console.log() // mostriamo tutte le risposte
```

----

Raccogliamo tramite prompt (eseguito tre volte) 3 parole dall'utente, per ogni parola ricevuta mostriamo in console "vocale" o "consonante" 
in base alla prima lettera. Usiamo un solo console.log per ogni parola sfruttando la potenzialità dell'operatore ternario.

--- 

Data una parola stampiamo in console la parola al rovescio. 
Per farlo prima usiamo il metodo split delle stringhe che trasforma una stringa in array e poi controlliamo se esiste un metodo per invertire gli elementi... 

```js 

constr string = prompt('...');

// controlliamo se è una stringa valida prima!

const array = string.split()

```

----


## Mercoledì 15/05
- AirBnB best practices: https://github.com/airbnb/javascript


### Esercizi

#### Nome e Cognome

- Chiediamo all'utente tramite un prompt di inserire il suo nome, poi salviamo il dato in una variabile;
- Chiediamo all'utente tramite un prompt di inserire il suo cognome, poi salviamo il dato in una variabile;

- Controlliamo che siano valori validi (non null), con almeno 3 caratteri e mostriamo tramite alert errori specifici;
- Se abbiamo mostrato un errore ricarichiamo la pagina usando `window.location.reload()`;

- Prendiamo il nome inserito e salviamo una nuova variabile trasformando la prima lettera in maiuscola, tip:

```js
    const firstName = '...';
    const firstLetter; // ...
    const nameWithoutFirstLetter; // ...
    const firstNaneWithCapitalize; // ...
```

- Prendiamo il cognome inserito e salviamo una nuova variabile trasformando la prima lettera in maiuscola;

- Mostriamo tramite alert "Ciao + [Nome] + [Cognome]"


#### Quizzone - Qui usiamo lo switch dove possibile

- Creiamo una variabile `let score = 0;`;
- Proponiamo all'utente, tramite prompt, 4 domande di cultura generale e raccogliamo le sue risposte in altrettante variabili;
- Per ogni risposta corretta aggiungiamo al `score` 3 punti, per ogni errata togliamo 1 punto;
- Alla fine delle 4 domande mostriamo il pungeggio complessivo;
- Poi se le hai indovinate tutte mostra un alert "Sei il nuovo campione!"

----


#### Esercizi 14/05

- definiamo variabile che contiene una stringa
    - Usiamo i doppi apici e salviamo la stringa: `Ciao Mondo!`
    - Usiamo i singoli apici e salviamo la stringa:` Mio zio viene dalla città di l'Aquila`
        - Occhio ad usare un escape per i singoli apici dentro la stringa!!
    - Usiamo il backtick per concatenare le due stringhe precendti dentro una nuova, usiamo anche "l'andata a capo" 

- Creiamo una nuova variabile in cui inseriamo una variabile precedente che modifichiamo portato il tutto in maiuscolo (`.toUpperCase()`) 
- Definiamo una variabile e salviamo all'interno un dato passato dall'utente tramite `prompt()`
    - Facciamo un console.log del dato precedento portato a lowercase

- Chiediamo al nostro user un numero da uno a 10 tramite prompt e solo se maggiore di 7 esclamare in console che ha vinto!
    - tips:

        ```js 
        prompt('Dammi un numero da uno a dieci!'); // occhio che il prompt torna una stringa!!
        if([...] > 7 ){

        }
        ```
