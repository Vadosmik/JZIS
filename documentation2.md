# 🧪 Dokumentacja laboratoriów

Zestawienie wykonanych laboratoriów z przedmiotu JZiS. Każdy wpis zawiera krótki opis, kod źródłowy oraz podgląd działania.

---

## 📋 Spis treści

- ⬅️ [Wróć do poprzedniej części: documentation1.md](documentation1.md)
- [Lab 6](#lab-6)
- [Lab 7](#lab-7)
- [Lab 8](#lab-8)
- [Lab 9](#lab-9)
- [Lab 10](#lab-10)

---

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
</details>

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

W tym laboratorium rozszerzyliśmy funkcjonalność formularza o walidację za pomocą JavaScript oraz dynamiczne wyświetlanie danych. Ćwiczenie składało się z trzech zadań:

1. **Walidacja pól formularza (wersja podstawowa)**  
   – Sprawdzenie, czy wszystkie pola tekstowe zostały wypełnione. Jeśli tak, po kliknięciu przycisku „Zapisz”, dane zostają wyświetlone obok pól.

2. **Walidacja rozszerzona**  
   – Oprócz poprzednich pól formularza dodano walidację m.in. dla: serii i numeru dowodu, kodu pocztowego, numeru domu.

3. **Kalkulator pierwiastków równania kwadratowego**  
   – Formularz do wprowadzenia współczynników równania kwadratowego oraz obliczenia pierwiastków.


### 🔧 Technologie  
`HTML`, `CSS`, `JavaScript`

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
                    <input type="text" id="pesel" name="pesel"><span id="pesel-out"></span><br>

                    <label for="nazwisko">Nazwisko</label>
                    <input type="text" id="nazwisko" name="nazwisko"><span id="nazwisko-out"></span><br>

                    <label for="imie">Imię</label>
                    <input type="text" id="imie" name="imie"><span id="imie-out"></span><br>

                    <label for="ulica">Ulica</label>
                    <input type="text" id="ulica" name="ulica"><span id="ulica-out"></span><br>

                    <label for="nr_domu">Nr domu / mieszkania</label>
                    <input type="text" id="nr_domu" name="nr_domu"><br>

                    <label for="kod">Kod pocztowy</label>
                    <input type="text" id="kod" name="kod"><br>

                    <label for="miasto">Miasto</label>
                    <input type="text" id="miasto" name="miasto"><span id="miasto-out"></span><br>

                    <label for="email">e-mail</label>
                    <input type="email" id="email" name="email"><br>
                </fieldset>

                <label for="email_odbioru">3. Informacja odbioru - email</label>
                <input type="checkbox" id="email_odbioru" name="email_odbioru"><br><br>

                <button type="button" onclick="pokaz_wartosc()" >Zapisz</button>
            </form>

            <p id="odp_for"></p>
        </section>
    </main>


    </fieldset>

    <footer>
        <p>© 2025 Twoja Przygoda. Wszystkie prawa zastrzeżone.</p>
    </footer>

</body>

<script src="script.js"></script>

</html>
```
</details>

<details>
<summary><strong>JavaScript</strong></summary>

```js


function pokaz_wartosc() {
    const inputy = document.querySelectorAll('form input[type="text"], form input[type="email"], form input[type="date"]');
    let nieWypelnione = [];

    inputy.forEach(input => {
        if (input.value.trim() === "") {
            nieWypelnione.push(input.name || input.id);
        }
    });

    if (nieWypelnione.length > 0) {
        alert("Uzupełnij wszystkie pola! Brakuje: " + nieWypelnione.join(", "));
        return;
    }

    // Jeśli wszystko wypełnione – można kontynuować
    document.getElementById("odp_for").innerHTML = "Wszystko poprawnie wypełnione!";

    const pola = ['pesel', 'nazwisko', 'imie', 'ulica', 'miasto'];
    pola.forEach(id => {
        const input = document.getElementById(id);
        const out = document.getElementById(id + '-out');
        out.textContent = ` → ${input.value}`;
    });
}




```

</details>

### kalkulator 
<details>
<summary><strong>HTML</strong></summary>

```html
<!DOCTYPE html>
<html lang="pl">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
    <title>Równanie Kwadratowe</title>
    <link rel="stylesheet" href="css/style.css" />
</head>
<body>

    <section class="form-container">
        <h2>Rozwiązywanie równania kwadratowego</h2>
        <form>
            <label for="a">Współczynnik a:</label>
            <input type="text" id="a" placeholder="np. 1" />

            <label for="b">Współczynnik b:</label>
            <input type="text" id="b" placeholder="np. -5" />

            <label for="c">Współczynnik c:</label>
            <input type="text" id="c" placeholder="np. 6" />

            <input type="button" id="przycisk" value="Oblicz" onclick="pokaz_wartosc()" />
        </form>

        <div id="wynik" class="wynik-pole">Tutaj pojawi się wynik...</div>
    </section>

    <script src="script.js"></script>
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

body {
    font-family: 'Segoe UI', sans-serif;
    background: linear-gradient(to right, #b2fefa, #0ed2f7);
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    padding: 20px;
}

.form-container {
    background-color: #ffffffdd;
    padding: 30px 40px;
    border-radius: 12px;
    box-shadow: 0 10px 20px rgba(0,0,0,0.1);
    width: 100%;
    max-width: 420px;
}

h2 {
    text-align: center;
    margin-bottom: 25px;
    color: #333;
}

form label {
    display: block;
    margin-top: 15px;
    font-weight: bold;
}

form input[type="text"] {
    width: 100%;
    padding: 10px;
    margin-top: 5px;
    border: 2px solid #ccc;
    border-radius: 8px;
    font-size: 16px;
}

form input[type="text"]:focus {
    border-color: #009688;
    outline: none;
}

input[type="button"] {
    margin-top: 20px;
    width: 100%;
    background-color: #007c91;
    color: #fff;
    padding: 12px;
    border: none;
    border-radius: 8px;
    font-size: 16px;
    font-weight: bold;
    cursor: pointer;
    transition: background-color 0.3s;
}

input[type="button"]:hover {
    background-color: #00bcd4;
}

.wynik-pole {
    margin-top: 25px;
    padding: 15px;
    background-color: #e0f2f1;
    border-left: 5px solid #007c91;
    border-radius: 8px;
    font-size: 16px;
    line-height: 1.5;
}

.blad {
    color: #d32f2f;
    font-weight: bold;
}
```

</details>

<details>
<summary><strong>JavaScript</strong></summary>

```js
function pokaz_wartosc() {
    const a = parseFloat(document.getElementById('a').value.trim());
    const b = parseFloat(document.getElementById('b').value.trim());
    const c = parseFloat(document.getElementById('c').value.trim());

    const wynikDiv = document.getElementById("wynik");

    if (isNaN(a) || isNaN(b) || isNaN(c)) {
        wynikDiv.innerHTML = `<span class="blad">Wszystkie pola muszą zawierać poprawne liczby!</span>`;
        return;
    }

    if (a === 0) {
        wynikDiv.innerHTML = `<span class="blad">To nie jest równanie kwadratowe (a ≠ 0)!</span>`;
        return;
    }

    const delta = b * b - 4 * a * c;
    let x1, x2;

    if (delta > 0) {
        x1 = (-b + Math.sqrt(delta)) / (2 * a);
        x2 = (-b - Math.sqrt(delta)) / (2 * a);
        wynikDiv.innerHTML = `
            <strong>Δ = ${delta.toFixed(2)}</strong><br>
            Dwa miejsca zerowe:<br>
            x₁ = ${x1.toFixed(2)}<br>
            x₂ = ${x2.toFixed(2)}
        `;
    } else if (delta === 0) {
        x1 = -b / (2 * a);
        wynikDiv.innerHTML = `
            <strong>Δ = ${delta.toFixed(2)}</strong><br>
            Jedno miejsce zerowe:<br>
            x = ${x1.toFixed(2)}
        `;
    } else {
        wynikDiv.innerHTML = `
            <strong>Δ = ${delta.toFixed(2)}</strong><br>
            Brak miejsc zerowych w zbiorze liczb rzeczywistych.
        `;
    }
}
```

</details>


### 🖼️ Podgląd
<img width="990" alt="Screenshot 2025-06-03 at 12 22 24" src="https://github.com/user-attachments/assets/4bd5935e-5e2d-4cbb-b6b8-1774d4514209" />

|   |   |
| ----------- | ----------- |
| <img width="591" alt="Screenshot 2025-06-03 at 12 24 40" src="https://github.com/user-attachments/assets/18c2bb34-df21-48d3-b861-dfb71e81b1c6" />| <img width="570" alt="Screenshot 2025-06-03 at 12 24 57" src="https://github.com/user-attachments/assets/27a2ae7a-918d-4e32-8f67-42f148299adf" />   |


---

## Lab 9

### 📄 Opis  

Laboratorium poświęcone było walidacji formularzy oraz prostym obliczeniom z wykorzystaniem JavaScript. Składało się z czterech zadań:

1. **Sprawdzenie poprawności logowania**  
   – Formularz z polami login, hasło i powtórz hasło. Walidacja obejmuje brak danych oraz porównanie haseł.

2. **Obliczanie wartości na podstawie ceny i ilości**  
   – Formularz, który sprawdza, czy cena i ilość zostały wprowadzone oraz czy są liczbami całkowitymi.

3. **Cena ze zniżką**  
   – Podobnie jak w zadaniu 2, z tym że po wpisaniu danych i kliknięciu przycisku obliczana jest cena z 30% zniżką.

4. **Formularz z pełną walidacją adresową**  
   – Rozbudowany formularz zawierający dane adresowe, datę urodzenia i login. Każde pole podlega walidacji, a obok wyświetlany jest komunikat (OK / Błąd / Nie wpisano).


### 🔧 Technologie  
`HTML`, `CSS`, `JavaScript`

### 💻 Kod

<details>
<summary><strong>Zadanie 1</strong></summary>
   <details>
<summary><strong>HTML</strong></summary>

```html
<!DOCTYPE html>
<html lang="pl">

<head>
    <meta charset="UTF-8">
    <link rel="stylesheet" href="style.css">
    <script type="text/javascript" src="skrypty.js"></script>
</head>

<body>

    <form>
        <label for="login">Login:</label><br>
        <input type="text" id="login" name="login" required><br><br>

        <label for="haslo">Hasło:</label><br>
        <input type="password" id="haslo" name="haslo" required><br><br>

        <label for="potwierdz">Potwierdź hasło:</label><br>
        <input type="password" id="potwierdz" name="potwierdz" required><br><br>

    </form>
    <button id="sprawdz" onclick="akcja()">Sprawdź</button>

    <div id="wyniki">
        <div id="wynik1"></div>
        <div id="wynik2"></div>
        <div id="wynik3"></div>
        <div id="wynik4"></div>
    </div>

</body>

</html>
```

</details>

<details>
<summary><strong>CSS</strong></summary>

```css
body {
    font-family: Arial, sans-serif;
    background-color: #f2f2f2;
    padding: 20px;
}

form {
    background-color: white;
    padding: 30px;
    border-radius: 8px;
    max-width: 300px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

label {
    font-weight: bold;
}

input[type="text"],
input[type="password"] {
    width: 90%;
    padding: 8px;
    margin-top: 4px;
    margin-bottom: 12px;
    border: 1px solid #ccc;
    border-radius: 4px;
}

button {
    padding: 10px 20px;
    background-color: #0078d7;
    color: white;
    border: none;
    border-radius: 4px;
    cursor: pointer;
    margin: 20px 0;
}

button:hover {
    background-color: #005fa3;
}

#wynik1, #wynik2, #wynik3 {
    margin-top: 5px;
    font-size: 14px;
}

#wynik1, #wynik2, #wynik3 {
    color: red;
}

#wynik4 {
    color: green;
}


#wyniki {
    width: 200px;
    padding: 10px;
    margin-top: 15px;
    font-size: 18px;
    font-weight: bold;
    background-color: #f0f0f0;
    border: 2px inset #ccc;
    border-radius: 8px;
    box-shadow: inset 2px 2px 5px rgba(0, 0, 0, 0.2),
                inset -2px -2px 5px rgba(255, 255, 255, 0.5);
}
```

</details>

<details>
<summary><strong>JavaScript</strong></summary>

```js
function akcja() {
    const login = document.getElementById('login').value.trim();
    const haslo = document.getElementById('haslo').value.trim();
    const potwierdz = document.getElementById('potwierdz').value.trim();

    const wynik1 = document.getElementById('wynik1');
    const wynik2 = document.getElementById('wynik2');
    const wynik3 = document.getElementById('wynik3');
    const wynik4 = document.getElementById('wynik4');

    wynik1.textContent = '';
    wynik2.textContent = '';
    wynik3.textContent = '';
    wynik4.textContent = '';

    let blad = false;

    if (login === '') {
        wynik1.textContent = 'Brak loginu';
        blad = true;
    }

    if (haslo === '') {
        wynik2.textContent = 'Brak hasła';
        blad = true;
    }

    if (potwierdz === '') {
        wynik3.textContent = 'Brak potwierdzenia hasła';
        blad = true;
    }

    if (!blad) {
        if (haslo !== potwierdz) {
            wynik3.textContent = 'Hasła są różne';
        } else {
            wynik4.textContent = 'Hasła są identyczne';
        }
    }
}
```

</details>
</details>

<details>
<summary><strong>Zadanie 2</strong></summary>
    <details>
    <summary><strong>HTML</strong></summary>

```html
<!DOCTYPE html>
<html lang="pl">

<head>
    <meta charset="UTF-8">
    <link rel="stylesheet" href="css/style.css">
    <script type="text/javascript" src="js/skrypty.js"></script>
</head>


<body>

    <form>
        <label for="liczba1">Podaj liczbę 1:</label><br>
        <input type="text" id="liczba1" name="liczba1" required><br><br>

        <label for="liczba2">Podaj liczbę 2:</label><br>
        <input type="text" id="liczba2" name="liczba2" required><br><br>

    </form>

    <button id="sprawdz" onclick="akcja()">Sprawdź</button>
    <div id="wynik"></div>

</body>

</html>
```
</details>

<details>
    <summary><strong>CSS</strong></summary>

```css
body {
    font-family: Arial, sans-serif;
    background-color: #f2f2f2;
    padding: 20px;
}

form {
    background-color: white;
    padding: 30px;
    border-radius: 8px;
    max-width: 300px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

label {
    font-weight: bold;
}

input[type="text"]{
    width: 90%;
    padding: 8px;
    margin-top: 4px;
    margin-bottom: 12px;
    border: 1px solid #ccc;
    border-radius: 4px;
}

button {
    padding: 10px 20px;
    background-color: #0078d7;
    color: white;
    border: none;
    border-radius: 4px;
    cursor: pointer;
    margin: 20px 0;
}

button:hover {
    background-color: #005fa3;
}

#wynik {
    height: 20px;
    width: 200px;
    padding: 10px;
    margin-top: 15px;
    font-size: 18px;
    font-weight: bold;
    background-color: #f0f0f0;
    border: 2px inset #ccc;
    border-radius: 8px;
    box-shadow: inset 2px 2px 5px rgba(0, 0, 0, 0.2),
                inset -2px -2px 5px rgba(255, 255, 255, 0.5);
}
```
</details>

<details>
    <summary><strong>JavaScript</strong></summary>

```js
function akcja() {
    const liczba1 = document.getElementById('liczba1').value.trim();
    const liczba2 = document.getElementById('liczba2').value.trim();
    const wynik = document.getElementById('wynik');

    wynik.textContent = '';

    if (liczba1 === '' || liczba2 === '') {
        wynik.textContent = 'Wpisz obie liczby.';
        return;
    }

    const a = parseFloat(liczba1);
    const b = parseFloat(liczba2);

    if (isNaN(a) || isNaN(b)) {
        wynik.textContent = 'Wprowadź prawidłowe liczby.';
        return;
    }

    const suma = a + b;
    wynik.textContent = `${a} + ${b} = ${suma}`;
}
```
</details>
</details>



<details>
<summary><strong>Zadanie 3</strong></summary>
    <details>
    <summary><strong>HTML</strong></summary>

    ```html
<!DOCTYPE html>
<html lang="pl">

<head>
    <meta charset="UTF-8">
    <link rel="stylesheet" href="css/style.css">
    <script type="text/javascript" src="js/skrypty.js"></script>
</head>


<body>

    <form>
        <label for="liczba1">cena:</label><br>
        <input type="text" id="liczba1" name="liczba1" required><br><br>

        <label for="liczba2">ilość:</label><br>
        <input type="text" id="liczba2" name="liczba2" required><br><br>

        <input type="checkbox" id="wybrano"><span>zniżka 30%</span>   

    </form>

    <button id="sprawdz" onclick="akcja()">Sprawdź</button>
    <div id="wynik"></div>

</body>

</html>
    ```
</details>

<details>
    <summary><strong>CSS</strong></summary>

    ```css
body {
    font-family: Arial, sans-serif;
    background-color: #f2f2f2;
    padding: 20px;
}

form {
    background-color: white;
    padding: 30px;
    border-radius: 8px;
    max-width: 300px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

label {
    font-weight: bold;
}

input[type="text"]{
    width: 90%;
    padding: 8px;
    margin-top: 4px;
    margin-bottom: 12px;
    border: 1px solid #ccc;
    border-radius: 4px;
}

button {
    padding: 10px 20px;
    background-color: #0078d7;
    color: white;
    border: none;
    border-radius: 4px;
    cursor: pointer;
    margin: 20px 0;
}

button:hover {
    background-color: #005fa3;
}

#wynik {
    height: 20px;
    width: 200px;
    padding: 10px;
    margin-top: 15px;
    font-size: 18px;
    font-weight: bold;
    background-color: #f0f0f0;
    border: 2px inset #ccc;
    border-radius: 8px;
    box-shadow: inset 2px 2px 5px rgba(0, 0, 0, 0.2),
                inset -2px -2px 5px rgba(255, 255, 255, 0.5);
}
    ```
</details>

<details>
    <summary><strong>JavaScript</strong></summary>

    ```js
function akcja() {
    const liczba1 = document.getElementById('liczba1').value.trim();
    const liczba2 = document.getElementById('liczba2').value.trim();
    const wybrano = document.getElementById('wybrano');
    const wynik = document.getElementById('wynik');

    wynik.textContent = '';

    if (liczba1 === '' || liczba2 === '') {
        wynik.textContent = 'Wpisz obie liczby.';
        return;
    }

    const a = parseFloat(liczba1);
    const b = parseFloat(liczba2);

    if (isNaN(a) || isNaN(b)) {
        wynik.textContent = 'Wprowadź prawidłowe liczby.';
        return;
    }

    if (!wybrano.checked) {
        const suma = a * b;
        wynik.textContent = `${suma}`;
    } else {
        const suma = (a * b) * 0.7;
        wynik.textContent = `${suma}`;
    }
}
    ```
</details>
</details>

<details>
<summary><strong>Zadanie 4</strong></summary>
    <details>
    <summary><strong>HTML</strong></summary>

    ```html
<!DOCTYPE html>
<html lang="pl">

<head>
    <meta charset="UTF-8">
    <link rel="stylesheet" href="css/style.css">
    <script type="text/javascript" src="js/skrypty.js"></script>
</head>


<body>

    <form>
        <label>Login:</label>
        <input type="text" id="login">
        <div id="loginInfo"></div><br>

        <label>Data urodzenia (DD-MM-RRRR):</label>
        <input type="text" id="data">
        <div id="dataInfo"></div><br>

        <label>Ulica:</label>
        <input type="text" id="ulica">
        <div id="ulicaInfo"></div><br>

        <label>Nr domu:</label>
        <input type="text" id="dom">
        <div id="domInfo"></div><br>

        <label>Nr lokalu:</label>
        <input type="text" id="lokal">
        <div id="lokalInfo"></div><br>

        <label>Kod pocztowy (XX-XXX):</label>
        <input type="text" id="kod">
        <div id="kodInfo"></div><br>

        <label>Miasto:</label>
        <input type="text" id="miasto">
        <div id="miastoInfo"></div><br>

    </form>

    <button id="sprawdz" onclick="waliduj()">Sprawdź</button>

</body>

</html>
    ```
</details>

<details>
    <summary><strong>CSS</strong></summary>

    ```css
body {
    font-family: Arial, sans-serif;
    background-color: #f2f2f2;
    padding: 20px;
}

form {
    background-color: white;
    padding: 30px;
    border-radius: 8px;
    max-width: 300px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

label {
    font-weight: bold;
}

input[type="text"]{
    width: 90%;
    padding: 8px;
    margin-top: 4px;
    margin-bottom: 12px;
    border: 1px solid #ccc;
    border-radius: 4px;
}

button {
    padding: 10px 20px;
    background-color: #0078d7;
    color: white;
    border: none;
    border-radius: 4px;
    cursor: pointer;
    margin: 20px 0;
}

button:hover {
    background-color: #005fa3;
}
    ```
</details>

<details>
    <summary><strong>JavaScript</strong></summary>

    ```js
function waliduj() {
  sprawdzPole("login", val => val !== "", "Nie wpisano");
  sprawdzPole("data", val => /^\d{2}-\d{2}-\d{4}$/.test(val), "Błąd");
  sprawdzPole("ulica", val => val !== "", "Nie wpisano");
  sprawdzPole("dom", val => val !== "", "Nie wpisano");
  sprawdzPole("lokal",  val => val !== "", "Nie wpisano");
  sprawdzPole("kod", val => /^\d{2}-\d{3}$/.test(val), "Błąd");
  sprawdzPole("miasto", val => val !== "", "Nie wpisano");
}

function sprawdzPole(id, walidacja, komunikatBledu = "Nie wpisano") {
  const el = document.getElementById(id);
  const info = document.getElementById(id + "Info");
  const wartosc = el.value.trim();

  if (wartosc === "" && komunikatBledu !== "Błąd") {
    info.textContent = komunikatBledu;
    info.style.color = "red";
  } else if (!walidacja(wartosc)) {
    info.textContent = komunikatBledu;
    info.style.color = "red";
  } else {
    info.textContent = "OK";
    info.style.color = "green";
  }
}
    ```
</details>
</details>

### 🖼️ Podgląd

|             |         |
|-------------|---------|
| <img width="471" alt="Screenshot 2025-06-03 at 13 00 42" src="https://github.com/user-attachments/assets/8f3891ea-b286-493a-a4e2-3518c4b002cd" /> | <img width="456" alt="Screenshot 2025-06-03 at 13 00 59" src="https://github.com/user-attachments/assets/40959eb5-409e-43b6-99ae-583dda006c71" /> |
| <img width="475" alt="Screenshot 2025-06-03 at 13 01 58" src="https://github.com/user-attachments/assets/7c94a06b-0f82-4ed9-b19c-f9c5dfa560cb" /> | <img width="447" alt="Screenshot 2025-06-03 at 13 02 17" src="https://github.com/user-attachments/assets/97086b89-8069-43af-b126-8933ad28eedd" /> |
| <img width="544" alt="Screenshot 2025-06-03 at 13 02 34" src="https://github.com/user-attachments/assets/f083b76a-e7ca-47fc-8534-d583efbcd89e" /> | <img width="451" alt="Screenshot 2025-06-03 at 13 02 46" src="https://github.com/user-attachments/assets/aca35de1-5909-46a1-8574-154dc170c8c7" /> |
| <img width="434" alt="Screenshot 2025-06-03 at 13 03 04" src="https://github.com/user-attachments/assets/31d82a12-d45d-4e53-acaa-bc857fad47f2" /> | <img width="407" alt="Screenshot 2025-06-03 at 13 03 43" src="https://github.com/user-attachments/assets/a9839381-0f60-4d9f-a7a8-2779f95a7d65" /> |
---

## Lab 10

### 📄 Opis  

Celem laboratorium było zapoznanie się z obsługą formularzy i zdarzeń w JavaScript. W skład ćwiczenia wchodziło pięć prostych interaktywnych zadań:

1. **Sprawdzenie pola tekstowego**  
   – Po kliknięciu przycisku pojawia się komunikat, czy użytkownik wprowadził dane.

2. **Obsługa checkboxów**  
   – Sprawdzenie, ile opcji zaznaczył użytkownik i odpowiedni komunikat w zależności od liczby zaznaczeń.

3. **Walidacja dwóch pól tekstowych**  
   – Informacja, czy oba pola zostały uzupełnione, jedno, czy żadne.

4. **Lista rozwijana (select)**  
   – Użytkownik wybiera kolor z listy, a po kliknięciu przycisku pojawia się nazwa wybranego koloru.

5. **Opcje radiowe (radio)**  
   – Po zatwierdzeniu wyboru pokazuje się, który wariant został zaznaczony.

### 🔧 Technologie  
`HTML`, `JavaScript`

### 💻 Kod

<details>
<summary>HTML <strong>zad 01</strong></summary>

```html
<!DOCTYPE html>
<html lang="pl">

<head>
  <meta charset="UTF-8">
  <title>Formularz danych</title>
</head>

<body>

  <form id="myForm">
    <input type="text" id="textInput" placeholder="Wpisz coś...">
    <button type="submit">Sprawdź</button>
  </form>

  <p id="message"></p>

  <script>
    document.getElementById('myForm').addEventListener('submit', function (event) {
      event.preventDefault();

      const input = document.getElementById('textInput').value.trim();
      const message = document.getElementById('message');

      if (input === "") {
        message.textContent = "Brak danych";
      } else {
        message.textContent = "Wprowadzono dane";
      }
    });
  </script>

</body>

</html>
```

</details>

<details>
<summary>HTML <strong>zad 02</strong></summary>

```html
<!DOCTYPE html>
<html lang="pl">

<head>
  <meta charset="UTF-8">
  <title>Formularz danych</title>
</head>

<body>

  <section>
    <form id="checkboxForm">
      <input type="checkbox" id="opc1"> Opcja 1<br>
      <input type="checkbox" id="opc2"> Opcja 2<br>
      <input type="checkbox" id="opc3"> Opcja 3<br><br>
      <button type="submit">Sprawdź</button>
      <div id="wynik"></div>
    </form>
  </section>

  <script>
    document.getElementById('checkboxForm').addEventListener('submit', function (event) {
      event.preventDefault();

      const opc1 = document.getElementById('opc1').checked;
      const opc2 = document.getElementById('opc2').checked;
      const opc3 = document.getElementById('opc3').checked;

      const zaznaczone = [opc1, opc2, opc3].filter(Boolean).length;

      const wynik = document.getElementById('wynik');

      if (zaznaczone === 0) {
        wynik.textContent = "Nic nie zaznaczono.";
      } else if (zaznaczone === 3) {
        wynik.textContent = "Wszystkie opcje zaznaczone.";
      } else {
        wynik.textContent = "Zaznaczono niepełny zestaw.";
      }
    });
  </script>

</body>

</html>
```

</details>

<details>
<summary>HTML <strong>zad 03</strong></summary>

```html
<!DOCTYPE html>
<html lang="pl">

<head>
  <meta charset="UTF-8">
  <title>Walidacja dwóch pól</title>
</head>

<body>

  <form id="formDane">
    <input type="text" id="pole1" placeholder="Pole 1"><br><br>
    <input type="text" id="pole2" placeholder="Pole 2"><br><br>
    <button type="submit">Sprawdź</button>
    <p id="komunikat"></p>
  </form>

  <script>
    document.getElementById('formDane').addEventListener('submit', function (event) {
      event.preventDefault();

      const p1 = document.getElementById('pole1').value.trim();
      const p2 = document.getElementById('pole2').value.trim();
      const komunikat = document.getElementById('komunikat');

      if (p1 === "" && p2 === "") {
        komunikat.textContent = "Oba pola nie są wypełnione";
      } else if (p1 === "" || p2 === "") {
        komunikat.textContent = "Jedno pole nie jest wypełnione";
      } else {
        komunikat.textContent = "Oba pola są wypełnione";
      }
    });
  </script>

</body>

</html>
```

</details>

<details>
<summary>HTML <strong>zad 04</strong></summary>

```html
<!DOCTYPE html>
<html lang="pl">

<head>
  <meta charset="UTF-8">
  <title>Wybór koloru</title>
</head>

<body>

  <label for="kolory">Wybierz kolor:</label><br>
  <select id="kolory">
    <option value="">-- wybierz --</option>
    <option value="Czerwony">Czerwony</option>
    <option value="Zielony">Zielony</option>
    <option value="Niebieski">Niebieski</option>
  </select>

  <button id="pokaz">Pokaż wybór</button><br><br>
  <span id="wynik"></span>

  <script>
    document.getElementById('pokaz').addEventListener('click', function () {
      const kolor = document.getElementById('kolory').value;
      const wynik = document.getElementById('wynik');
      wynik.textContent = "Wybrano: " + kolor;
    });
  </script>

</body>

</html>
```

</details>

<details>
<summary>HTML <strong>zad 05</strong></summary>

```html
<!DOCTYPE html>
<html lang="pl">

<head>
  <meta charset="UTF-8">
  <title>Wybór opcję</title>
</head>

<body>

  <form id="formularzWariant">
    <p>Wybierz opcję:</p>
    <input type="radio" id="wariant1" name="wariant" value="Wariant A">
    <label for="wariant1">Opcja A</label><br>

    <input type="radio" id="wariant2" name="wariant" value="Wariant B">
    <label for="wariant2">Opcja B</label><br>

    <input type="radio" id="wariant3" name="wariant" value="Wariant C">
    <label for="wariant3">Opcja C</label><br><br>

    <button type="submit">Zatwierdź</button>
  </form>

  <div id="wynik"></div>

  <script>
    document.getElementById('formularzWariant').addEventListener('submit', function (event) {
      event.preventDefault();

      const wybrany = document.querySelector('input[name="wariant"]:checked');
      const wynik = document.getElementById('wynik');

      if (wybrany) {
        wynik.textContent = "Wybrano: " + wybrany.value;
      } else {
        wynik.textContent = "Nie wybrano żadnego wariantu.";
      }
    });
  </script>

</body>

</html>
```

</details>

### 🖼️ Podgląd
<img width="363" alt="Screenshot 2025-06-03 at 12 38 03" src="https://github.com/user-attachments/assets/d6257317-61cb-46b9-8b50-58b96cbd240a" />

---

## Lab 11

### 📄 Opis  

Celem laboratorium było przygotowanie do kolokwium poprzez stworzenie kompletnego układu strony internetowej (layoutu) oraz implementację formularza z walidacją po stronie klienta za pomocą JavaScript.

Strona została zaprojektowana zgodnie z podanym wzorem graficznym i składała się z czterech głównych sekcji:

- **Nagłówek (`header`)** – stała wysokość 80px, pełna szerokość (1000px),
- **Panel środkowy (`main`)** – zawierał formularz z polami do wypełnienia,
- **Panel boczny (`aside`)** – dodatkowe informacje, np. linki lub ogłoszenia,
- **Stopka (`footer`)** – o takich samych wymiarach jak nagłówek.

Layout strony był statyczny i wyśrodkowany w przeglądarce, o wymiarach 1000 × 600 pikseli.

Formularz w panelu głównym zawierał pola:

- imię (tekst),
- email (adres e-mail),
- wiek (liczba całkowita 1–120),
- PESEL (dokładnie 11 cyfr),
- przycisk „Wyślij”.

### 🔧 Technologie  
`HTML`, `CSS`, `JavaScript`

### 💻 Kod

<details>
<summary><strong>HTML</strong></summary>

```html
<!DOCTYPE html>
<html lang="pl">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>lab 11</title>
    <link rel="stylesheet" href="css/style.css">
     <script src="js/script.js"></script> 
</head>

<body>

    <content>
        <header>
            <h1>Rozbudowany Formularz</h1>
        </header>

        <main>
            <h2>Dane uzytkownika</h2>
            <form action="" method="post">
                <label for="name">Imię:</label>
                <input type="text" id="name" name="name">
                <label for="nameError"></label>

                <label for="email">Email:</label>
                <input type="email" id="email" name="email">
                <label for="emailError"></label>

                <label for="age">Wiek:</label>
                <input type="number" id="age" name="age">
                <label for="ageError"></label>

                <label for="pesel">PESEL:</label>
                <input type="number" id="pesel" name="pesel">
                <label for="peselError"></label>

                <button type="submit">Wyślij</button>
            </form>
        </main>
        <aside>
            <h3>Panel boczny</h3>
            <p>Mozesz tu dodac np. informacje kontaktowe, linki lub ogtoszenia.</p>
        </aside>
        <footer>
            <p>Stopka strony - przyktadowy tekst</p>
        </footer>
    </content>

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

body {
    height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
}

content {
    display: grid;
    grid-template-columns: 666px 334px;
    grid-template-rows: 80px 440px 80px;
    grid-template-areas:
        "header header"
        "main aside"
        "footer footer";
    box-shadow: #505947 0px 0px 10px;
}

/* === HEADER === */

header {
    grid-area: header;
    background-color: #4F709C;
    display: flex;
    align-items: center;
    justify-content: center;
}

/* === MAIN === */

main {
    grid-area: main;
    padding: 2rem;
}

main h2 {
    margin-bottom: 1rem;
}

form {
    display: grid;
    grid-template-columns: auto 1fr 1fr;
    gap: 0.5rem 1rem;
    align-items: center;
    max-width: 600px;
}

label:not([for$="Error"]) {
    font-weight: bold;
}

input {
    padding: 0.5rem;
    border: 1px solid #aaa;
    font-size: 1rem;
    width: 200px;
}

label[for$="Error"] {
    font-size: 0.85rem;
    color: red;
    min-height: 1em;
}

button {
    padding: 0.75rem;
    font-size: 1rem;
    cursor: pointer;
    border: none;
    background-color: #c0c0c0;
}

/* === ASIDE === */
aside {
    grid-area: aside;
    background-color: #BF7F5A;
    padding: 20px;
}

/* === FOOTER === */
footer {
    grid-area: footer;
    background-color: #505947;
    display: flex;
    align-items: center;
    justify-content: center;
}
```

</details>

<details>
<summary><strong>JavaScript</strong></summary>

```js
document.addEventListener("DOMContentLoaded", function () {
    const form = document.querySelector("form");

    form.addEventListener("submit", function (e) {
        e.preventDefault();
        let valid = true;

        clearErrors()

        const name = document.getElementById("name").value.trim();
        const email = document.getElementById("email").value.trim();
        const age = document.getElementById("age").value.trim();
        const pesel = document.getElementById("pesel").value.trim();

        if (name === "") {
            valid = false;
            showError("nameError", "Imię jest wymagane");
        }

        if (email === "") {
            valid = false;
            showError("emailError", "Email jest wymagany");
        }

        const ageNum = parseInt(age);
        if (!Number.isInteger(ageNum) || ageNum < 1 || ageNum > 120) {
            valid = false;
            showError("ageError", "Wiek musi być liczbą całkowitą od 1 do 120");
        }

        if (!/^\d{11}$/.test(pesel)) {
            valid = false;
            showError("peselError", "PESEL musi zawierać dokładnie 11 cyfr");
        }

        if (valid) {
            alert(`Dane użytkownika:
                - Imię: ${name}
                - Email: ${email}
                - Wiek: ${ageNum}
                - PESEL: ${pesel}`);
        }
    });

    function showError(labelId, message) {
        const label = document.querySelector(`label[for="${labelId}"]`);
        label.textContent = message;
        label.style.color = "red";
        label.style.fontSize = "0.9em";
    }
    function clearErrors() {
        const errorLabels = ["nameError", "emailError", "ageError", "peselError"];
        errorLabels.forEach(id => {
            const label = document.querySelector(`label[for="${id}"]`);
            if (label) label.textContent = "";
        });
    }
});
```

</details>

### 🖼️ Podgląd
<img width="1101" alt="Screenshot 2025-06-03 at 12 33 54" src="https://github.com/user-attachments/assets/f344d738-dc89-4c7e-95c6-0381c9fdda2b" />
<img width="1090" alt="Screenshot 2025-06-03 at 12 34 12" src="https://github.com/user-attachments/assets/2ea531dc-8040-4ba5-aa4c-2a01f2accdbe" />

---
