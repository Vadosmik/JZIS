## Lab 6

### 📄 Opis  
W ramach laboratorium rozszerzyliśmy projekt z Lab 3 o funkcjonalność wielu podstron oraz stylizację nawigacji. Celem ćwiczenia było zorganizowanie zawartości w postaci osobnych stron oraz implementacja prostego systemu nawigacyjnego.

Zadania obejmowały:

1. **Dodanie dwóch podstron**  
   – Stworzenie osobnych plików HTML i przeniesienie na nie wybranych informacji z głównej strony.

2. **Nawigacja między stronami**  
   – Dodanie `navbar`a z odnośnikami umożliwiającymi przechodzenie między stronami.

3. **Stylizacja `navbar`a**  
   – Zastosowanie efektu `hover`, który zmieniał tło przycisków na obrazek.

4. **Struktura listy**  
   – Przerobienie `navbar`a tak, by był zbudowany z listy (`<ul><li>`), co poprawia semantykę i ułatwia dalsze stylowanie.

Zadanie miało na celu zapoznanie się z wielostronicową strukturą witryny, organizacją plików oraz podstawami interaktywnego i estetycznego projektowania nawigacji.

w kodzie niżej umiesciłem tylko kod 3 zadania bo 4 i 3 jest to same tylko ze zmiana stylu navbar a w 3 mnie strona podoba sie liepiej

### 🔧 Technologie  
`HTML`, `CSS`

### 💻 Kod

<details>
<summary><strong>HTML</strong></summary>

```html
<!DOCTYPE html>
<html lang="pl">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Twoja Przygoda – Odkryj Świat</title>
    <link rel="stylesheet" href="css/style.css">
</head>

<body>
    <img id="header-img" src="https://b2ccdn.coraltravel.pl/content/banner/desktop/bannerslide_12032025134349.jpg"
        alt="Podróże - baner">

    <header>
        <h1>Twoja Przygoda – Odkryj Świat z Nami!</h1>
        <nav>
            <ul>
                <li><a href="index.html">Strona główna</a></li>
                <li><a href="Podstrona1.html">Najlepsze kierunki podróży</a></li>
                <li><a href="Podstrona2.html">Porady podróżnicze</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section id="home">
            <h2>Witaj na naszej stronie podróżniczej!</h2>
            <p>Podróże to nie tylko przemieszczanie się – to styl życia. Odkryj z nami najpiękniejsze miejsca na
                świecie!</p>
        </section>

        <section id="about">
            <h2>O nas</h2>
            <p>Podróże to nasza pasja! Jesteśmy zespołem miłośników odkrywania świata, którzy chcą dzielić się z Tobą
                najlepszymi miejscami, poradami i inspiracjami. Dołącz do naszej społeczności i zacznij swoją przygodę!
            </p>
        </section>

        <section id="contact">
            <h2>Kontakt</h2>
            <p>Masz pytania? Skontaktuj się z nami! Chętnie pomożemy w zaplanowaniu Twojej wymarzonej podróży.</p>
        </section>
    </main>

    <footer>
        <p>© 2025 Twoja Przygoda. Wszystkie prawa zastrzeżone.</p>
    </footer>

</body>

</html>
```

</details>

<details>
<summary><strong>Podstrona 1</strong></summary>

```html
<!DOCTYPE html>
<html lang="pl">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Twoja Przygoda – Odkryj Świat</title>
    <link rel="stylesheet" href="css/style.css">
</head>

<body>
    <img id="header-img" src="https://b2ccdn.coraltravel.pl/content/banner/desktop/bannerslide_12032025134349.jpg"
        alt="Podróże - baner">

        <header>
            <h1>Twoja Przygoda – Odkryj Świat z Nami!</h1>
            <nav>
                <ul>
                    <li><a href="index.html">Strona główna</a></li>
                    <li><a href="Podstrona1.html">Najlepsze kierunki podróży</a></li>
                    <li><a href="Podstrona2.html">Porady podróżnicze</a></li>
                </ul>
            </nav>
        </header>

    <main>

        <section id="destinations">
            <h2>Najlepsze kierunki podróży</h2>
            <article>
                <img src="img/bali.jpeg" alt="Bali">
                <span>
                    <h3>Bali – Rajska wyspa pełna magii</h3>
                    <p>Odkryj piękne plaże, tropikalne dżungle i kulturę Bali. Sprawdź najlepsze miejsca do odwiedzenia!
                    </p>
                </span>
            </article>
            <article>
                <span>
                    <h3>Paryż – Miasto Miłości i Sztuki</h3>
                    <p>Wieża Eiffla, Luwr, kawiarnie i romantyczna atmosfera – zobacz, dlaczego Paryż zachwyca turystów!
                    </p>
                </span>
                <img src="img/paryz.jpeg" alt="Paryż">
            </article>
            <article>
                <img src="img/islandia.jpeg" alt="Islandia">
                <span>
                    <h3>Islandia – Kraina lodu i ognia</h3>
                    <p>Gorące źródła, lodowce i zorza polarna – Islandia to miejsce, które musisz zobaczyć na własne
                        oczy!</p>
                </span>
            </article>
        </section>
    </main>

    <footer>
        <p>© 2025 Twoja Przygoda. Wszystkie prawa zastrzeżone.</p>
    </footer>

</body>

</html>
```

</details>

<details>
<summary><strong>Podstrona 2</strong></summary>

```html
<!DOCTYPE html>
<html lang="pl">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Twoja Przygoda – Odkryj Świat</title>
    <link rel="stylesheet" href="css/style.css">
</head>

<body>
    <img id="header-img" src="https://b2ccdn.coraltravel.pl/content/banner/desktop/bannerslide_12032025134349.jpg"
        alt="Podróże - baner">

        <header>
            <h1>Twoja Przygoda – Odkryj Świat z Nami!</h1>
            <nav>
                <ul>
                    <li><a href="index.html">Strona główna</a></li>
                    <li><a href="Podstrona1.html">Najlepsze kierunki podróży</a></li>
                    <li><a href="Podstrona2.html">Porady podróżnicze</a></li>
                </ul>
            </nav>
        </header>

    <main>

        <section id="tips">
            <h2>Porady podróżnicze</h2>
        
            <article>
                <h3>Jak pakować się na każdą podróż?</h3>
                <p>Sprawdź nasz poradnik minimalisty – co zabrać, a czego unikać!</p>
            </article>
        
            <article>
                <h3>Najlepsze aplikacje dla podróżników</h3>
                <p>Mapy offline, przewodniki i tłumacze – oto aplikacje, które ułatwią Ci życie!</p>
            </article>
        
            <article>
                <h3>Bezpieczne podróżowanie – na co uważać?</h3>
                <p>Dowiedz się, jak zabezpieczyć dokumenty, unikać oszustw i podróżować bezpiecznie niezależnie od celu.</p>
            </article>
        
            <article>
                <h3>Jak unikać jet lagu?</h3>
                <p>Podpowiadamy, jak przystosować się do zmiany strefy czasowej i cieszyć się podróżą bez zmęczenia.</p>
            </article>
        
            <article>
                <h3>Podróżowanie z ograniczonym budżetem</h3>
                <p>Dowiedz się, jak oszczędzać na noclegach, jedzeniu i atrakcjach – bez rezygnowania z jakości wyprawy!</p>
            </article>
        
            <article>
                <h3>Zdrowie w podróży – co warto zabrać?</h3>
                <p>Apteczka, ubezpieczenie, szczepienia – o tych rzeczach nie możesz zapomnieć, planując wyjazd!</p>
            </article>
        </section>

    </main>

    <footer>
        <p>© 2025 Twoja Przygoda. Wszystkie prawa zastrzeżone.</p>
    </footer>

</body>

</html>
```

</details>

<details>
<summary><strong>CSS</strong></summary>

```css
/* 

W elemencie article img i article span zastosowano float: left;, aby obraz wyrównywał się do lewej strony i pozwalał tekstowi opływać go z prawej. 
Dodatkowo w article dodano overflow: hidden;, aby zapobiec problemom z opływaniem (float), 
które mogłyby powodować przesunięcie lub niepoprawne rozmieszczenie zawartości. 

*/

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

#header-img {
    width: 1000px;
    height: 300px;
    object-position: bottom right;
    object-fit: cover;
    display: block;
}

body {
    font-family: Arial, sans-serif;
    background-color: #e0f7fa;
    color: #333;
    margin: 0;
    padding: 0;
    display: flex;
    flex-direction: column;
    align-items: center;
}

.container {
    width: 1000px;
    max-width: 100%;
}

header {
    background: #ff7043;
    color: white;
    text-align: center;
    padding: 20px 10px;
    width: 1000px;
    height: 205px;
    max-width: 100%;
    box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.2);
}

header h1 {
    font-size: 28px;
    margin-bottom: 10px;
}

nav ul {
    list-style: none;
}

nav ul li {
    margin: 5px 0;
}

nav ul li a {
    color: white;
    text-decoration: none;
    font-weight: bold;
    padding: 12px 20px;
    background: #ff9800;
    border-radius: 8px;
    background-image:url(../img/off.png);
    background-size: cover;
    transition: background 0.3s, transform 0.2s;
    display: inline-block;
}

nav ul li a:hover {
    background: #fb8c00;
    background-image:url(../img/on.png);
    background-size: cover;
    transform: scale(1.05);
}

main {
    width: 1000px;
    max-width: 100%;
    padding: 30px;
    display: flex;
    flex-direction: column;
    align-items: center;
}

section {
    width: 100%;
    margin-bottom: 30px;
    padding: 20px;
    background: #fff3e0;
    border-radius: 8px;
    box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.1);
    text-align: center;
}

section h2 {
    font-size: 26px;
    margin-bottom: 20px;
    color: #ff7043;
    border-bottom: 3px solid #ff7043;
    display: inline-block;
    padding-bottom: 5px;
}

article {
    width: 100%;
    overflow: hidden;
    background: #ffebee;
    padding: 20px;
    margin-bottom: 15px;
    border-radius: 8px;
    text-align: left;
    transition: transform 0.2s;
}

article:hover {
    transform: scale(1.02);
}

article img {
    float: left;
    border-radius: 5px;
    width: 150px;
    height: 150px;
    object-fit: cover;
    margin-right: 15px; /* Dystans między obrazem a tekstem */
}

article span {
    overflow: hidden;
    float: left;
    width: calc(100% - 165px);
}

article h3 {
    color: #d32f2f;
    margin-bottom: 8px;
}

footer {
    height: 50px;
    width: 1000px;
    max-width: 100%;
    background: #333;
    color: white;
    text-align: center;
    padding: 20px;
    font-size: 14px;
    margin-top: 20px;
    box-shadow: 0px -4px 8px rgba(0, 0, 0, 0.2);
}
```

### 🖼️ Podgląd

<img width="222" alt="Screenshot 2025-05-28 at 22 36 08" src="https://github.com/user-attachments/assets/d883874b-82a8-420b-8357-0b1b77abab08" />
<img width="1095" alt="Screenshot 2025-05-28 at 22 36 32" src="https://github.com/user-attachments/assets/99931933-fd69-4ee2-8fad-8cd9d8996dc8" />

---

## Lab 7

### 📄 Opis  
W tym laboratorium stworzyliśmy prosty formularz przy użyciu wyłącznie HTML i CSS. Celem ćwiczenia było poznanie struktury formularza oraz elementów służących do zbierania danych od użytkownika.

Do zbudowania formularza wykorzystano:

- znacznik `<form>` do zdefiniowania formularza,
- `<fieldset>` i `<legend>` do grupowania powiązanych pól,
- `<input>`, `<label>`, `<textarea>` oraz `<select>` do tworzenia różnych typów pól wejściowych.

Dodatkowo formularz został ostylowany z użyciem CSS, m.in. poprzez nadanie marginesów, kolorów i wyrównania, aby zwiększyć jego czytelność i estetykę. Formularz nie zawierał jeszcze logiki — był jedynie strukturą wizualną.

### 🔧 Technologie  
`HTML`, `CSS`

### 💻 Kod

<details>
<summary><strong>HTML</strong></summary>

```html
<!DOCTYPE html>
<html lang="pl">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Twoja Przygoda – Odkryj Świat</title>
    <link rel="stylesheet" href="css/style.css">
</head>

<body>
    <img id="header-img" src="https://b2ccdn.coraltravel.pl/content/banner/desktop/bannerslide_12032025134349.jpg"
        alt="Podróże - baner">

    <header>
        <h1>Twoja Przygoda – Odkryj Świat z Nami!</h1>
        <nav>
            <a href="index.html">Strona główna</a>
            <a href="Podstrona1.html">Najlepsze kierunki podróży</a>
            <a href="Podstrona2.html">Porady podróżnicze</a>
            <a href="formularz.html">formularz</a>
        </nav>
    </header>

    <!--    Formularz    -->

    <main>
        <section>
            <h2>WNIOSEK</h2>
            <form>

                <section class="data">
                    <label for="data">Data wypełnienia wniosku</label>
                    <input type="date" id="data" name="data_wniosku">
                </section>

                <fieldset>
                    <legend>1. Dane wniosku i dowodu</legend>
                    <label for="nr_wniosku">Numer wniosku</label>
                    <input type="text" id="nr_wniosku" name="nr_wniosku"><br>

                    <label for="seria">Seria dowodu i numer dowodu</label>
                    <input type="text" id="seria" name="seria_dowodu" class="seria">
                
                    <label for="numer_dowodu">-</label>
                    <input type="text" id="numer_dowodu" name="numer_dowodu">
                </fieldset>

                <fieldset>
                    <legend>2. Dane posiadacza dowodu</legend>
                    <label for="pesel">Numer PESEL</label>
                    <input type="text" id="pesel" name="pesel"><br>

                    <label for="nazwisko">Nazwisko</label>
                    <input type="text" id="nazwisko" name="nazwisko"><br>

                    <label for="imie">Imię</label>
                    <input type="text" id="imie" name="imie"><br>

                    <label for="ulica">Ulica</label>
                    <input type="text" id="ulica" name="ulica"><br>

                    <label for="nr_domu">Nr domu / mieszkania</label>
                    <input type="text" id="nr_domu" name="nr_domu"><br>

                    <label for="kod">Kod pocztowy</label>
                    <input type="text" id="kod" name="kod"><br>

                    <label for="miasto">Miasto</label>
                    <input type="text" id="miasto" name="miasto"><br>

                    <label for="email">e-mail</label>
                    <input type="email" id="email" name="email"><br>
                </fieldset>

                <label for="email_odbioru">3. Informacja odbioru - email</label>
                <input type="email" id="email_odbioru" name="email_odbioru"><br><br>

                <button type="submit">Zapisz</button>
            </form>
        </section>
    </main>


    </fieldset>

    <footer>
        <p>© 2025 Twoja Przygoda. Wszystkie prawa zastrzeżone.</p>
    </footer>

</body>

</html>
```

</details>

<details>
<summary><strong>CSS</strong></summary>

```css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

#header-img {
    width: 1000px;
    height: 300px;
    object-position: bottom right;
    object-fit: cover;
    display: block;
}

body {
    font-family: Arial, sans-serif;
    background-color: #e0f7fa;
    color: #333;
    margin: 0;
    padding: 0;
    display: flex;
    flex-direction: column;
    align-items: center;
}

.container {
    width: 1000px;
    max-width: 100%;
}

header {
    background: #ff7043;
    color: white;
    text-align: center;
    padding: 20px 10px;
    width: 1000px;
    height: 125px;
    max-width: 100%;
    box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.2);
}

header h1 {
    font-size: 28px;
    margin-bottom: 10px;
}

nav {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 15px;
    margin-top: 15px;
}

nav a {
    color: white;
    text-decoration: none;
    font-weight: bold;
    padding: 12px 20px;
    background: #ff9800;
    border-radius: 8px;
    background-image:url(../img/off.png);
    background-size: cover;
    transition: background 0.3s, transform 0.2s;
    display: inline-block;
}

nav a:hover {
    background: #fb8c00;
    background-image:url(../img/on.png);
    background-size: cover;
    transform: scale(1.05);
}

main {
    width: 1000px;
    max-width: 100%;
    padding: 30px;
    display: flex;
    flex-direction: column;
    align-items: center;
}

section {
    width: 100%;
    margin-bottom: 30px;
    padding: 20px;
    background: #fff3e0;
    border-radius: 8px;
    box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.1);
    text-align: center;
}

section h2 {
    font-size: 26px;
    margin-bottom: 20px;
    color: #ff7043;
    border-bottom: 3px solid #ff7043;
    display: inline-block;
    padding-bottom: 5px;
}

article {
    width: 100%;
    overflow: hidden;
    background: #ffebee;
    padding: 20px;
    margin-bottom: 15px;
    border-radius: 8px;
    text-align: left;
    transition: transform 0.2s;
}

article:hover {
    transform: scale(1.02);
}

article img {
    float: left;
    border-radius: 5px;
    width: 150px;
    height: 150px;
    object-fit: cover;
    margin-right: 15px; /* Dystans między obrazem a tekstem */
}

article span {
    overflow: hidden;
    float: left;
    width: calc(100% - 165px);
}

article h3 {
    color: #d32f2f;
    margin-bottom: 8px;
}

footer {
    height: 50px;
    width: 1000px;
    max-width: 100%;
    background: #333;
    color: white;
    text-align: center;
    padding: 20px;
    font-size: 14px;
    margin-top: 20px;
    box-shadow: 0px -4px 8px rgba(0, 0, 0, 0.2);
}

/* formularz */

form fieldset {
    border: none;
    border-top: 1px solid black;
    margin-bottom: 2rem;
    padding: 20px 30% 20px 0;
    position:relative;

    text-align: right;
}

legend {
    font-weight: bold;
    margin-bottom: 1rem;
    display: block;
    float: left;
    
    position:absolute;
    top:-25px;
    left:0px;
}

label {
    margin-top: 1rem;
}

input[type="text"],
input[type="email"],
input[type="date"] {
  width: 225px;
  padding: 0.5rem;
  margin-top: 0.25rem;
  border: 1px solid #ccc;
  border-radius: 0.5rem;
}

section.data,
section.podwojne {
background: none;
box-shadow: none;
}

button {
    display: block;
    margin: auto;
    padding: 0.75rem 2rem;
    background: #007bff;
    color: white;
    border: none;
    border-radius: 0.5rem;
    font-size: 1rem;
    cursor: pointer;
  }

  button:hover {
    background: #0056b3;
  }

section.data {
  position: relative;
  top: 0;
  right: 0;
  text-align: right;
}

  .seria {
    max-width: 50px;
  }
```

</details>


### 🖼️ Podgląd

<img width="1087" alt="Screenshot 2025-05-28 at 22 43 27" src="https://github.com/user-attachments/assets/912551ff-0c8c-438e-81bf-04666f6e9c35" />

---

## Lab 8

### 📄 Opis  
P

### 🔧 Technologie  
`HTML`, `CSS`, `JavaScript`

### 💻 Kod

<details>
<summary><strong>HTML</strong></summary>

```html

```

</details>

<details>
<summary><strong>CSS</strong></summary>

```css

```

</details>

<details>
<summary><strong>JavaScript</strong></summary>

```js

```

</details>

### 🖼️ Podgląd

---

## Lab 9

### 📄 Opis  
P

### 🔧 Technologie  
`HTML`, `CSS`, `JavaScript`

### 💻 Kod

<details>
<summary><strong>HTML</strong></summary>

```html

```

</details>

<details>
<summary><strong>CSS</strong></summary>

```css

```

</details>

<details>
<summary><strong>JavaScript</strong></summary>

```js

```

</details>

### 🖼️ Podgląd

---

## Lab 10

### 📄 Opis  
P

### 🔧 Technologie  
`HTML`, `CSS`, `JavaScript`

### 💻 Kod

<details>
<summary><strong>HTML</strong></summary>

```html

```

</details>

<details>
<summary><strong>CSS</strong></summary>

```css

```

</details>

<details>
<summary><strong>JavaScript</strong></summary>

```js

```

</details>

### 🖼️ Podgląd
