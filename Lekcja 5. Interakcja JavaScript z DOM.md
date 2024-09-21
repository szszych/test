# Interakcja JavaScript z DOM

## Jak JavaScript współpracuje z DOM?

JavaScript może zmieniać treści i elementy na stronie dzięki DOM. Korzystając z różnych metod, możemy znaleźć, zmodyfikować lub usunąć elementy strony.

Oto kilka przykładów interakcji JavaScriptu z **DOM**, które pomogą lepiej zrozumieć, jak można dynamicznie manipulować stroną internetową.

### 1. **Zmienianie atrybutów elementów**

Możesz zmieniać atrybuty elementów HTML, takie jak `src` dla obrazów lub `href` dla linków.

#### Przykład zmiany obrazu:
```javascript
let image = document.querySelector('img');
image.setAttribute('src', 'nowe_zdjecie.jpg');
image.setAttribute('alt', 'Opis nowego zdjęcia');
```

#### Przykład zmiany linku:
```javascript
let link = document.querySelector('a');
link.setAttribute('href', 'https://nowyadres.pl');
link.textContent = 'Odwiedź nową stronę!';
```

### 2. **Dodawanie i usuwanie klas CSS**

Możesz dodawać lub usuwać klasy CSS, aby dynamicznie zmieniać styl elementów na stronie.

#### Przykład dodania klasy:
```javascript
let element = document.querySelector('div');
element.classList.add('highlight');
```

#### Przykład usunięcia klasy:
```javascript
element.classList.remove('highlight');
```

#### Przykład przełączania klasy (toggle):
Jeśli klasa już istnieje, zostanie usunięta. Jeśli jej nie ma, zostanie dodana.
```javascript
element.classList.toggle('highlight');
```

### 3. **Tworzenie nowych elementów**

Możesz dynamicznie tworzyć nowe elementy na stronie i dodawać je do DOM.

#### Przykład dodania nowego przycisku:
```javascript
let newButton = document.createElement('button');
newButton.textContent = 'Kliknij mnie!';
document.body.appendChild(newButton);
```

### 4. **Usuwanie elementów**

Możesz także usuwać elementy z DOM za pomocą JavaScript.

#### Przykład usunięcia elementu:
```javascript
let elementToRemove = document.querySelector('#do-usuniecia');
elementToRemove.remove();
```

### 5. **Zmiana stylów elementów**

Możesz dynamicznie zmieniać style elementów poprzez dostęp do właściwości `style`.

#### Przykład zmiany koloru i rozmiaru tekstu:
```javascript
let paragraph = document.querySelector('p');
paragraph.style.color = 'red';
paragraph.style.fontSize = '20px';
```

### 6. **Obsługa zdarzeń**

JavaScript może reagować na różne zdarzenia, takie jak kliknięcia, najechanie kursorem lub zmiana wartości w polu formularza.

#### Przykład zdarzenia kliknięcia:
```javascript
let button = document.querySelector('button');
button.addEventListener('click', function() {
    alert('Przycisk został kliknięty!');
});
```

#### Przykład zdarzenia najechania myszką:
```javascript
let image = document.querySelector('img');
image.addEventListener('mouseover', function() {
    image.style.border = '5px solid green';
});
```

#### Przykład zdarzenia zmiany wartości w polu tekstowym:
```javascript
let input = document.querySelector('input');
input.addEventListener('input', function() {
    console.log('Wartość pola tekstowego to: ' + input.value);
});
```

### 7. **Manipulowanie formularzami**

JavaScript umożliwia obsługę formularzy i walidację danych przed ich wysłaniem.

#### Przykład pobrania wartości z pola formularza:
```javascript
let form = document.querySelector('form');
form.addEventListener('submit', function(event) {
    event.preventDefault();  // Zapobiega domyślnemu wysłaniu formularza
    let username = document.querySelector('#username').value;
    console.log('Nazwa użytkownika: ' + username);
});
```

### 8. **Animacja elementów przy użyciu CSS**

Możesz dodawać proste animacje za pomocą zmiany wartości stylów w określonym czasie.

#### Przykład zmiany pozycji elementu:
```javascript
let box = document.querySelector('.box');
let position = 0;
function moveBox() {
    position += 1;
    box.style.left = position + 'px';
    if (position < 300) {
        requestAnimationFrame(moveBox);
    }
}
moveBox();
```

### 9. **Tworzenie listy dynamicznie**

Możesz tworzyć całe listy i dodawać je do strony w czasie rzeczywistym.

#### Przykład dodania listy elementów:
```javascript
let fruits = ['Jabłko', 'Banana', 'Gruszka'];
let ul = document.createElement('ul');

fruits.forEach(function(fruit) {
    let li = document.createElement('li');
    li.textContent = fruit;
    ul.appendChild(li);
});

document.body.appendChild(ul);
```

### 10. **Znajdowanie wielu elementów i iteracja po nich**

Możesz pobierać wiele elementów naraz i wykonać na nich operacje.

#### Przykład zmiany koloru tekstu w wielu elementach:
```javascript
let paragraphs = document.querySelectorAll('p');
paragraphs.forEach(function(p) {
    p.style.color = 'blue';
});
```

### Podsumowanie

Interakcja JavaScriptu z DOM pozwala na dynamiczne zmiany na stronie internetowej, takie jak dodawanie nowych elementów, zmiana treści, stylów, a także reagowanie na różne działania użytkownika. Dzięki temu można budować interaktywne i nowoczesne strony oraz aplikacje webowe.
