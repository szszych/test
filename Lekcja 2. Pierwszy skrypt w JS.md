# Początek.

Zaczniemy od pracy z JavaScriptem po stronie klienta, a dokładnie z JS w środowisku przeglądarki.

Instrukcja pracy z konsolą JavaScript w Google Chrome
Konsola JavaScript w Google Chrome to narzędzie dla programistów, które umożliwia interakcję z kodem JavaScript na stronie internetowej. Umożliwia ona testowanie kodu, debugowanie oraz wyświetlanie komunikatów o błędach i logów.

1. Otwieranie konsoli
   Aby otworzyć konsolę JavaScript w Google Chrome, możesz wykonać jeden z poniższych kroków:

Skrót klawiaturowy: Naciśnij klawisz F12 lub Ctrl + Shift + I (Windows) / Cmd + Option + I (Mac), aby otworzyć narzędzia deweloperskie, a następnie przejdź do zakładki Console.
Menu przeglądarki: Kliknij w menu (trzy kropki w prawym górnym rogu przeglądarki) -> Więcej narzędzi -> Narzędzia dla programistów -> zakładka Console.
2. Podstawowe operacje w konsoli
Wyświetlanie wiadomości: Możesz użyć polecenia console.log(), aby wyświetlać wiadomości w konsoli. Wpisz poniższy kod i naciśnij Enter:

```javascript
console.log('Witaj w konsoli JavaScript!');
Efekt: W konsoli pojawi się wiadomość "Witaj w konsoli JavaScript!".
```

Wykonywanie operacji matematycznych: Możesz bezpośrednio wykonywać operacje matematyczne w konsoli.

```javascript
2 + 2
Efekt: Konsola wyświetli wynik 4.
```

Definiowanie zmiennych i funkcji: Możesz deklarować zmienne i tworzyć funkcje bezpośrednio w konsoli.

```javascript
let x = 5;
let y = 10;
console.log(x + y); // Wynik to 15
```

3. Debugowanie kodu
   Konsola pozwala na wyświetlanie błędów, ostrzeżeń i innych ważnych informacji:

Wyświetlanie błędów: Jeśli w kodzie JavaScript pojawi się błąd, zostanie on automatycznie wyświetlony w konsoli.

Ręczne wyrzucenie błędu: Możesz ręcznie wygenerować błąd za pomocą polecenia console.error().

```javascript
console.error('To jest komunikat o błędzie');
```

Wyświetlanie ostrzeżeń: Za pomocą console.warn() można wyświetlić ostrzeżenie w konsoli.

```javascript
console.warn('To jest ostrzeżenie!');
```

4. Sprawdzanie elementów DOM
   Konsola umożliwia również bezpośrednią manipulację i sprawdzanie elementów strony internetowej:

Pobieranie elementów HTML: Możesz pobierać elementy z DOM przy użyciu JavaScript.

```javascript
let header = document.querySelector('h1');
console.log(header);
```

Zmiana treści elementu: Możesz również zmieniać zawartość elementów.

```javascript
header.textContent = "Zmieniono tekst nagłówka!";
```


5. Czyszczenie konsoli
Jeśli chcesz wyczyścić konsolę, użyj polecenia:

```javascript
console.clear();
```

To usunie wszystkie wcześniejsze komunikaty i informacje wyświetlone w konsoli.

6. Używanie skrótów w konsoli
   Strzałki w górę/w dół: Pozwalają na przeglądanie poprzednich komend.
   Tab: Użyj klawisza Tab, aby automatycznie uzupełniać nazwę zmiennej lub funkcji.
7. Monitorowanie wydajności
   Konsola Chrome oferuje także polecenia do monitorowania wydajności kodu:

console.time() i console.timeEnd(): Służą do mierzenia czasu wykonania kodu.

```javascript
console.time('Test');
// Kod, który chcesz przetestować
console.timeEnd('Test');
```

Dodatkowe funkcje

8. Interakcja z kodem na stronie: Możesz wykonywać dowolne skrypty JavaScript na stronie w czasie rzeczywistym, bez konieczności edytowania kodu źródłowego.
   Inspekcja elementów: Możesz kliknąć prawym przyciskiem myszy na dowolny element strony i wybrać "Zbadaj", aby otworzyć narzędzia deweloperskie i zobaczyć element w konsoli.
   Konsola JavaScript w Google Chrome to potężne narzędzie, które umożliwia szybkie debugowanie, testowanie oraz interakcję z kodem strony.
