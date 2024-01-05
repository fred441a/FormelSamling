# programmerings paradimer
## Dynamic programming
Dynamic programming er er programming uden recursion. Dette er ofte opnået ved at loope igennem en funktion flere gange og gemme resultaterne. Ofte resultere dette i en hurtigere algoritme da man kan gemme resultatet for flere funktions kald som ville give det samme resultat istedet for at køre funktionen flere gange

### subproblem graf (afhængligheds graf)
et recursivt problem kan beskrives som et problem med flere subproblemer. den originale funktion afhænger af løsningen af disse subproblemer. En subproblem graf viser os hvilket subproblem der ikke afhænger af nogle andre, og dermed hvilen rækkefølge subproblemerne skal løsses i.

fx hvis vi havde koden.

```
function fibonachi (int n){
    if (n == 0){
        return 0;
    }
    if (n == 1){
        return 1;
    }
    return fibonachi(n-1)+fibonachi(n-2)
}
```

hvis n = 5 fåes subproblem grafen:

![Subptoblem graf](https://i.imgur.com/UYALrtc.png)

## Greedy algorithms
En greedy algoritme der "gårdigt" vælger hvad der virker som den bedste løsning lokalt, for forhåbenligt at komme til den bedste generelle løsning.

## Divide and Conquer
Ved denne metode løses et eller uoverskueligt problem ved at dele det op, løse undederlene og derefter ligge resultatet sammen.
