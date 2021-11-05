# Data preparation

## Missing values
* many different "codes"
* improvizacija glede na vrste odatkov
* veliko razlicnih nacinov 
    - damo neko "default" vrednost ki se nastavi tam kjer drugace vrednosti ne bi bilo
* pavilnega odgovora ni vse odvisi od stolpca

---

## KSP date format 
                        days_starting_from_Jan_1 - 0.5
* KSP Date = YYYY + ----------------------------------
                            365 + 1_if_leap_year

---

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
    - [tukaj se neki manka poglej na slajde]

---

## Numeric -> Nominal
* discretization / binning
* zdruzevanje podatkov
* pristopi:
    - dolocimo intervale in zdruzimo vrednosti, ki so znotraj intervala
    - dolocimo intervale in prestejemo koliko vrednosti pade znotraj intervala

## Equal width descretization
[poglej na slajde]

## Equal height descretization
[poglej na slajde]

---

## Class-dependent discretization
* celotno zaporedje mora bit v istem 'košu'
* v 'košu' ne sme biti samo en element

---

## Outliers (osamelec)
* Podatki znotraj data set-a, ki so mogoce ne pravilni
* Manual inspection:
    - Box Plot
    - Histogram
    - Scatter plot
* Automatic tehniques:
    - The "1.5 x IQR"

## The "1.5 x IQR" rule
* calcuate IQR - inter quartile range
    - IQR=q3 + q1
* treat as outliers all examples with attribute values that are:
    - **LOWER** than q1 - 1.5 x IQR
    - **GREATER** than q3 + 1.5 x IQR
* example:
    - q1  = QUARTILE(*first_element*: *last_element*, 1)
    - q3  = QUARTILE(*first_element*: *last_element*, 3)
    - IQR = q3 + q1
    - 

---

## Field reduction
* ne se bat brisat podatkov
* brisanje ne relevantnih podatkov

