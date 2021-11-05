# Data preparation

## Missing values
    * many different "codes"
    * improvizacija glede na vrste odatkov
    * veliko razlicnih nacinov 
        - damo neko "default" vrednost ki se nastavi tam kjer drugace vrednosti ne bi bilo
    * pavilnega odgovora ni vse odvisi od stolpca

## KSP date format 
                          days_starting_from_Jan_1 - 0.5
    * KSP Date = YYYY + ----------------------------------
                              365 + 1_if_leap_year
     
## Nominal -> Numeric
    * Nominal: podatki, ki niso v stevilski obliki
    * Kako narediti pretvorbo:
        - Two nominal values/options (binary) -> change to 0 and 1
            - example: STATUS: open door / closed door
                       nominal -> numeric: open door = 1
                                           closed door = 0
        - More than two values:
            - Ordered -> preserve the order
            - Unordered -> every value gets it's own 0-1 attribute
        -  
