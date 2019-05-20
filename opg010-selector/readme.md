# CSS Selector opgave

Dette er en simpel opgave i brugen af forskellige CSS selectors.

Start med at skabe en HTML side med følgende opmærkninger (bare kopier):

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

    <p>This is p-opmærkning #1</p>
    <p>This is p-opmærkning #2</p>
    <p>This is p-opmærkning #3</p>
    <p id="myP1">This is p-opmærkning #4 with an id-value of "myP1"</p>
    <p id="myP2">This is p-opmærkning #5 with an id-value of "myP2"</p>
    <p class="myClass1">This is p-opmærkning #6 with an class-value of "myClass1"</p>
    <p class="myClass2">This is p-opmærkning #7 with an class-value of "myClass2"</p>
    <p class="myClass1 myClass2">This is p-opmærkning #8 with an class-value of "myClass1 myClass2"</p>
    <div>
      <p>This is p-opmærkning #9 in a div</p>
    </div>
    <div id="div1">
      <p>This is p-opmærkning #10 in a div with id-value of "div1"</p>
    </div>
    <div id="div2" class="myClass3">
      <p>This is p-opmærkning #11 in a div with class-value of "myClass3"</p>
    </div>
    <p>This is a ul</p>
    <ul>
      Item 1
      Item 2
      Item 3
    </ul>

    <div>
      <p>This is a ul in a div</p>
      <ul>
        Item 1
        Item 2
        Item 3
        Item 4
        Item 5
      </ul>
    </div>
    <p>This is an image with a title-attributte</p>
    <img title="my title" src="https://www.w3.org/2015/10/W3C-Developers_Assets/W3C-Developers-Dark.png" alt="image" width="100" />
    <p>This is an image without a title-attributte</p>
    <img src="https://www.w3.org/2015/10/W3C-Developers_Assets/W3C-Developers-Dark.png" alt="image" width="100" />
    <p>This is an image without a alt-value of "W3C image"</p>
    <img src="https://www.w3.org/2015/10/W3C-Developers_Assets/W3C-Developers-Dark.png" alt="W3C image" width="100" />

    <p>This is a textbox</p>
    <input type="text" />

    <p>This is a checkbox</p>
    <input type="checkbox" />
  </body>
</html>
```

Du kan også kopiere [herfra](index.html)

Du skal nu åbne F12-toolet, åbne konsolen, og finde elementer ved hjælp af $$ (find flere elementer) - eksempelvis:

```
$$("p")
```

burde finde og vise Allee p-opmærkninger.

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
