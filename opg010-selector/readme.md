# CSS Selector opgave

Dette er en simpel opgave i brugen af forskellige CSS selectors.

Start med at skabe en HTML side med [disse opmærkninger](index.html).

Du skal nu åbne F12-toolet, åbne konsolen, og finde elementer ved hjælp af $$ (find flere elementer) - eksempelvis:

```
$$("p")
```

burde finde og vise alle p-opmærkninger.

Prøv at se om du kan finde følgende:

- Alle p-opmærkninger
- Alle images-opmærkninger 
- Alle p-opmærkninger og images 
- p-opmærkning med en id = myP1
- p-opmærkninger med en id = myP1 eller id = myP1
- p-opmærkning med en class = myClass1 
- p-opmærkning med en class = myClass2 eller myClass2 
- Alle p-opmærkninger under div-opmærknings
- Alle p-opmærkninger under div med id = div1
- Alle p-opmærkninger under div med class = myClass3
- Alle ul 
- Alle li under ul
- Alle images med en title attribut
- Alle images hvor alt-opmærkning indeholder "W3C"
- Alle textboxes 
- Alle checkboxes
- Den første li in hver ul 

## Løsning

- $$("p")
- $$("img")
- $$("p, img")
- $$("#myP1") or $$("p#myP1")
- $$("#myP1, #myP2")
- $$(".myClass1") or $$("p.myClass1")
- $$(".myClass1.myClass2")
- $$("p div")
- $$("div#div1 p")
- $$("div.myClass3 p")
- $$("ul")
- $$("ul li")
- $$("img[title]")
- $$("img[alt*='W3C']")
- $$("input[type='text']")
- $$("input[type='checkbox']")
- $$("ul li:first-child")
