# ID.3 -> C4.5
* 1993/94
* V weki J.48

## Kaj c4.5 nadgrajuje nad id.3
1. numerični atribution
2. mankajoče vrednosti
3. Šum / rezanje
    a) postpruning - predhodno
    b) prepruning  - naknadno

## Numerični atributi
* določimo neko mejo
* in damo v eno množico vrednosti manjže od meje
* in v drugo množico damo vrednosti večje od meje
 
## Mankajoče vrednosti 
* Oznaka "?"
* En način: Smatramo mankajoco vrednost kot loceno vrednost
* Mankajoce vrednosti c4.5 uporabi pri gradnji drevesa

## Rezanje
* To prevent overfitting
* Naknadno rezanje - zgradimo celotno drevo in nato pogledamo kaj bi se lahko dalo porezati

### Predhodno rezanje

### Naknadno rezanje
* zgradimo celotno drevo
* Moznosti:
    #### 1. Zamenjava
     * od dna gor
     * lahko zamenjamo celotno sub-drevo z listom ~ porezemo

    #### 2. Povzdvigovanje
     * Neko podrevo ki je bilo nizje ga dvignemo visje v drevo

## Ocenjevanje napake pri rezanju
* rezemo samo ce bo zmanjsalo napako
* 