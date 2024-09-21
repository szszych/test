### Struktura dokumentu HTML

Każdy dokument HTML składa się z zestawu elementów, które tworzą hierarchię, podobnie jak drzewo. Każdy element ma określoną rolę w organizowaniu treści i struktury strony internetowej. Poniżej znajdziesz omówienie głównych elementów dokumentu HTML.

#### 1. **Deklaracja DOCTYPE**
   ```html
   <!DOCTYPE html>
   ```
   - Deklaracja DOCTYPE informuje przeglądarkę, że dokument jest napisany w języku HTML5.

#### 2. **Element `<html>`**
   ```html
   <html lang="pl">
   <!-- Zawartość strony -->
   </html>
   ```
   - Zawiera cały dokument HTML. Atrybut `lang="pl"` informuje przeglądarki i wyszukiwarki, że językiem treści strony jest polski.

#### 3. **Element `<head>`**
   ```html
   <head>
       <meta charset="UTF-8">
       <title>Tytuł Strony</title>
   </head>
   ```
   - Zawiera metadane strony, czyli informacje, które nie są bezpośrednio widoczne na stronie, ale mają kluczowe znaczenie dla przeglądarek i wyszukiwarek.
   - **`<meta charset="UTF-8">`** – Określa kodowanie znaków, co zapewnia poprawne wyświetlanie polskich znaków.
   - **`<title>`** – Tytuł strony, wyświetlany na karcie przeglądarki.

#### 4. **Element `<body>`**
   ```html
   <body>
       <h1>Witaj na mojej stronie!</h1>
       <p>To jest paragraf z tekstem.</p>
   </body>
   ```
   - Zawiera treść strony, czyli wszystko, co użytkownik widzi na stronie: teksty, obrazy, linki, filmy, formularze, itp.
   - **`<h1>`** – Nagłówek główny, który jest zazwyczaj największym i najważniejszym tekstem na stronie.
   - **`<p>`** – Paragraf, który zawiera bloki tekstu.

### Przykład kompletnego dokumentu HTML:

```html
<!DOCTYPE html>
<html lang="pl">
  <head>
    <meta charset="UTF-8">
    <title>Moja Pierwsza Strona</title>
  </head>
  <body>
    <h1>Witaj na mojej stronie!</h1>
    <p>To jest przykładowy paragraf z tekstem.</p>
  </body>
</html>
```

#### Główne części dokumentu HTML:

1. **Deklaracja DOCTYPE** – Informuje przeglądarkę, że to dokument HTML5.
2. **Element `<html>`** – Obejmuje cały dokument HTML.
3. **Element `<head>`** – Zawiera metadane, takie jak kodowanie znaków i tytuł strony.
4. **Element `<body>`** – Zawiera widoczną treść strony, czyli tekst, obrazy i inne elementy wyświetlane użytkownikowi.

Taka struktura HTML pozwala przeglądarce na poprawne renderowanie strony i jej elementów, co zapewnia dobrą organizację oraz przejrzystość treści.