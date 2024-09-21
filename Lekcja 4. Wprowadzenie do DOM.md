# Wprowadzenie do DOM

## 1. Co to jest DOM?

**DOM (Document Object Model)** to sposób, w jaki przeglądarka organizuje strukturę strony HTML. Zamienia ona elementy strony (takie jak nagłówki, paragrafy, linki) na strukturę drzewa, która jest dostępna dla JavaScriptu. Dzięki DOM, JavaScript może dynamicznie manipulować stroną, zmieniać treść, dodawać nowe elementy lub usuwać istniejące.

## 2. Jak wygląda struktura DOM?

Wyobraź sobie stronę HTML w formie drzewa. Każdy element HTML to gałąź drzewa, a każdy tekst czy atrybut to liść.

Przykład prostego HTML:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Tytuł Strony</title>
  </head>
  <body>
    <h1>Witaj na stronie!</h1>
    <p>To jest paragraf.</p>
  </body>
</html>
```

Przekształca się w drzewo DOM:

```bash
#document
   └── html
       ├── head
       │   └── title
       │       └── "Tytuł Strony"
       └── body
           ├── h1
           │   └── "Witaj na stronie!"
           └── p
               └── "To jest paragraf."
```

Każdy element HTML (np.`<html>`, `<head>`, `<body>`) staje się węzłem w drzewie DOM, a JavaScript może modyfikować te węzły.

## 3. Dlaczego DOM jest ważny?

DOM pozwala na dynamiczne zmiany na stronie bez przeładowania. Dzięki niemu możemy:

* zmieniać teksty na stronie
* dodawać lub usuwać elementy
* reagować na działania użytkownika (np. kliknięcia)
* zmieniać style (kolory, rozmiary itp.)



Przykład: W DOM możemy zmienić zawartość nagłówka na stronie bez przeładowania strony.
```javascript
document.querySelector('h1').textContent = "Zmieniono nagłówek!";
```
