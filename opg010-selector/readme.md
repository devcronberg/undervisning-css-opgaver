# CSS Selector opgave

Dette er en simpel opgave i brugen af forskellige CSS selectors.

Start med at skabe en HTML side med disse opmærkninger:

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Min app</title>
  </head>
  <body>
    <h1>CSS Selector</h1>

    <p>p-tag #1</p>
    <p>p-tag #2</p>
    <p>p-tag #3</p>
    <p id="myP1">p-tag #4 med id "myP1"</p>
    <p id="myP2">p-tag #5 med id "myP2"</p>
    <p class="myClass1">p-tag #6 med class "myClass1"</p>
    <p class="myClass2">p-tag #7 med class "myClass2"</p>
    <p class="myClass1 myClass2">p-tag #8 med class "myClass1 myClass2"</p>
    <div>
      <p>p-tag #9 i en div</p>
    </div>
    <div id="div1">
      <p>p-tag #10 i en div med id "div1"</p>
    </div>
    <div id="div2" class="myClass3">
      <p>p-tag #11 i en div med class "myClass3"</p>
    </div>
    <p>Her kommer en ul</p>
    <ul>
      <li>Item 1</li>
      <li>Item 2</li>
      <li>Item 3</li>
    </ul>

    <div>
      <p>Her er en ul i en div</p>
      <ul>
        <li>Item 1</li>
        <li>Item 2</li>
        <li>Item 3</li>
        <li>Item 4</li>
        <li>Item 5</li>
      </ul>
    </div>
    <p>Billede med en title-attributte</p>
    <img title="my title" src="https://www.w3.org/2015/10/W3C-Developers_Assets/W3C-Developers-Dark.png" alt="image" width="100" />
    <p>Billede uden en title-attributte</p>
    <img src="https://www.w3.org/2015/10/W3C-Developers_Assets/W3C-Developers-Dark.png" alt="image" width="100" />
    <p>Billede med en alt-value "W3C image"</p>
    <img src="https://www.w3.org/2015/10/W3C-Developers_Assets/W3C-Developers-Dark.png" alt="W3C image" width="100" />

    <p>textbox</p>
    <input type="text" />

    <p>checkbox</p>
    <input type="checkbox" />
  </body>
</html>

```

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
- p-opmærkninger med en id = myP1 eller id = myP2
- p-opmærkning med en class = myClass1 
- p-opmærkning med en class = myClass1 eller myClass2 
- Alle p-opmærkninger under div-opmærkninger
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
- $$("#myP1") --- eller  $$("p#myP1")
- $$("#myP1, #myP2")
- $$(".myClass1") --- eller $$("p.myClass1")
- $$(".myClass1.myClass2")
- $$("div p")
- $$("div#div1 p")
- $$("div.myClass3 p")
- $$("ul")
- $$("ul li")
- $$("img[title]")
- $$("img[alt*='W3C']")
- $$("input[type='text']")
- $$("input[type='checkbox']")
- $$("ul li:first-child")
