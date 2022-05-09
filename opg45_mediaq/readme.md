# Brug af media queries

I denne opgave skal du prøve at lege lidt med media queries. Med udgangspunkt i følgende html:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <link rel="stylesheet" href="style.css" />
    <title>Document</title>
  </head>
  <body>
    <div class="center">Lorem ipsum</div>
  </body>
</html>
```

og følgende css

```css
div {
  width: 400px;
  height: 400px;
  font-size: 2em;
  background-color: pink;
}

.center {
  line-height: 400px;
  height: 400px;
  border: 3px solid green;
  text-align: center;
}
```

Din opgave er at sørge for, at firkanten ændrer farve afhængig af størrelsen på browseren:

- op til 600px = pink
- min 600px = red
- min 800px = blue
- min 1000px = yellow

Du kan bruge dette som skabelon

```css
@media only screen and (min-width: [xxx]px) {
  div {
    background-color: [color];
  }
}
```

Se evt min løsning - [html](index.html) og [css](style.css).
