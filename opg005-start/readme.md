# Start på CSS

I denne opgave skal du tilknytte CSS til et dokument. Start med at oprette et nyt HTML dokument med følgende indhold:

```html
<!DOCTYPE html>
<html lang="da">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS</title>
</head>

<body>
    <h1>CSS</h1>    
</body>
</html>
```
## Ekstern CSS

Prøv nu at skabe et nyt CSS dokument kaldet style.css med følgende indhold:

```css
h1{
    color: blue;
}
```

og sørg for at dokumentet er linket til HTML dokumentet i head-opmærkningen med:

```html
<link rel="stylesheet" href="style.css">
```

Se HTML siden gennem Live Server - hvad farve har overskriften? Den skulle gerne være blå. Se også F12-toolet ved at højreklikke på overskriften og vælge "Inspect/Undersøg". Kan du se at overskrift er blå og har overskrevet browserens eget style sheet?

## Intern CSS

Tilføj nu følgende i head-opmærkning efter førnævnte link:

```html
<style>
    h1{
        color: green;
    }
</style>
```

Se HTML siden gennem Live Server - hvad farve har overskriften? Den skulle gerne være grøn. Se også F12-toolet ved at højreklikke på overskriften og vælge "Inspect/Undersøg". Kan du se at overskrift er grøn, og har overskrevet både det eksterne og browserens eget style sheet?

## Rækkefølge

Prøv at bytte om på link- og style-opmærkningen - hvad farve er overskriften nu? Se også F12-toolet.

## Inline CSS

Ret overskriften til følgende:

```html
<h1 style="color: red">CSS</h1> 
```

Se HTML siden gennem Live Server - hvad farve har overskriften? Den skulle gerne være rød. Se også F12-toolet ved at højreklikke på overskriften og vælge "Inspect/Undersøg". Kan du se at overskrift er rød, og har overskrevet både det eksterne, interne og browserens eget style sheet?

Se evt [min løsning](index.html).