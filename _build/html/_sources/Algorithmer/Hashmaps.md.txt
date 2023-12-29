# Hashmaps / Hash tables
Hashmaps er en datastruktur hvor posistionen af dataen i memory er beskrevet gennem en funktion.

## key
det data der beskriver inputtet i din hashing funktion

## index mapping ( trivial hashing )
beskriver hashing functionen f(x)=x altså er din key lig med posistionen i memory

## collision
hvis en funktion retunere den samme område i memory ved 2 forskellige keys

## seperate chaining
en måde at løse collisions problemer ved at erstate indgangen i memory med en liste som indeholde begge værdier der skal være på denne key.

## Open addressing
open adressing betyder at din indang i hastabellen ikke behøver at være det præcise resultat af hash functionen. Når man ændre på hvilken posistion noget ligger på kalder man det probing

## linear probing
en probing methode hvor man bare tager den næste frie plads i memory

## quadratic probing ( mid-square method )
her søger man igennem index+x² hvor x stiger med 1 indtil man finder en plads
