# 🧪 Dokumentacja laboratoriów

Zestawienie wykonanych laboratoriów z przedmiotu JZiS. Każdy wpis zawiera krótki opis, kod źródłowy oraz podgląd działania.

---

## 📋 Spis treści

- [Lab 1](#lab-1)
- [Lab 2](#lab-2)
- [Lab 3](#lab-3)
- [Lab 4](#lab-4)
- [Lab 5](#lab-5)
- ➡️ [Przejdź do kolejnej części: documentation2.md](documentation2.md)

---

## Lab 1

### 📄 Opis  
Celem było stworzenie strony z podanego zdj, było podane 2 zdj prostych stron z opisem uczelni i formularzem trzeba było zrobić str które były by podobne na te zdj

### 🔧 Technologie  
`HTML`, `CSS`

### 💻 Kod

<details>
<summary><strong>HTML1</strong></summary>

```html
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="author" content="Mikanovich Vadzim">
    <title>UMG Formulaż</title>
    <script type="text/javascript" nonce="19436f72e03846cb91b32bc5bbe" src="//local.adguard.org?ts=1748460873584&amp;type=content-script&amp;dmn=ilias.umg.edu.pl&amp;url=https%3A%2F%2Filias.umg.edu.pl%2Filias.php%3Fref_id%3D113168%26ass_id%3D12025%26_table_nav%3Dfiletitle%3Aasc%3A0%26delivered%3D186054%26cmd%3Ddownload%26cmdClass%3Dilexsubmissionfilegui%26cmdNode%3Dxu%3A131%3Axz%3A139%26baseClass%3DilExerciseHandlerGUI&amp;app=com.apple.Safari&amp;css=3&amp;js=1&amp;rel=1&amp;rji=1&amp;sbe=1"></script>
<script type="text/javascript" nonce="19436f72e03846cb91b32bc5bbe" src="//local.adguard.org?ts=1748460873584&amp;name=AdGuard%20Extra&amp;type=user-script"></script><link rel="stylesheet" href="style.css">
</head>

<body>
<div>
    <img src="umg-zolty.png">
    <span class="headName">Uniwersytet Morski w Gdyni   </span>
    <img src="budynekUMG.jpg">
</div>

<h2>Krótka charakterystyka uczelni</h2>
<p>Uniwersytet Morski w Gdyni jest uczelnią kształcącą i wychowującą przyszłych oficerów marynarki handlowej, wysoko wykwalifikowanych specjalistów w zakresie eksploatacji statków, portów, zarządzania systemem transportowym oraz innych specjalistów gospodarki morskiej na poziomie inżynierskim i magisterskim.</p>

<table>
    <tr>
       <td>
        <div>
            <p>Obecnie w ciagu jednego roku akademickiego w UMG kształci się:</p>
            <ul>
                <li>ponad 5000 studentów dziennych,</li>
                <li>2500 oficerów i marynarzy,</li>
                <li>5000 członków załóg w Fundacji Rozwoju UM w Gdyni.</li>
            </ul>
        </div>
       </td> 
        <td>
            <img src="dar.jpg">
            <img src="horyzont.jpg">
        </td>
    </tr>
</table>


<h2>Wydziały</h2>
<p>Uniwersytet Morski w Gdyni kształci studentów na czterech wydziałach:</p>
        <ul>
            <li>Wydział Elektryczny</li>
            <li>Wydział Mechaniczny</li>
            <li>Wydział Nawigacyjny</li>
            <li>Wydział Przedsiębiorczości i Towaroznawstwa</li>
        </ul>
<p><a href="umg_formulaz.html">Zarejestruj się</a>, aby otrzymywać informacje na temat studiów w UMG.</p>
    
<h2>Historia uczelni</h2>
<table class="history">
    <tr>
       <td>12 VI 1920</td> <td>Departament do Spraw Morskich Ministrstwa Spraw Wojskowych wyanonsował 247 000 dolarów na zkup i remont trzymasztowego żaglowca "Nest", przeznaczonego na statek dla Szkoły Morskiej w Tczewie.</td>
    </tr>
    <tr>
       <td>17 VI 1920</td> <td>Minister Spraw Wojskowych gen. Józef Leśniewski podpisał akt utworzenia Szkoły Morskiej w Tczewie. Szkoła miała na początku dwa wydziały Nawigacyjny i Mechaniczny</td>
    </tr>
    <tr>
       <td>15 VII 1920</td> <td>Pierwsze egzaminy zdawano z matematyki, geografii, języka obcego i kreślenia. Po egzaminach wstępnych uczniowie poszli prosto na wojnę polsko-bolszewicką. Uroczystości otwarcia odbyły się dopiero po zakończeniu działń wojennych.</td>
    </tr>
    <tr>
       <td>8 XII 1920</td> <td>Uroczyste otwarcie SM w Tczewie.</td>
    </tr>
    <tr>
       <td>4 IX 1921</td> <td>Wyremontowany żaglowiec "Nest" otrzymał nazwę "Lwów" i banderę.</td>
    </tr>
    <tr>
       <td>1 I 1922</td> <td>Szkoła Morska przeszła pod władzę Departamentu Marynarki Handlowej Ministerstwa Przemysłu i Handlu i stała się uczelnią typu cywilnego.</td>
    </tr>
    <tr>
       <td> ... </td> <td> ... </td>
    </tr>
 </table>



</body>
</html>
```

</details>

<details>
<summary><strong>HTML2</strong></summary>

```html
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <title>UMG Formulaż</title>
    <script type="text/javascript" nonce="19436f72e03846cb91b32bc5bbe" src="//local.adguard.org?ts=1748460873584&amp;type=content-script&amp;dmn=ilias.umg.edu.pl&amp;url=https%3A%2F%2Filias.umg.edu.pl%2Filias.php%3Fref_id%3D113168%26ass_id%3D12025%26_table_nav%3Dfiletitle%3Aasc%3A0%26delivered%3D186055%26cmd%3Ddownload%26cmdClass%3Dilexsubmissionfilegui%26cmdNode%3Dxu%3A131%3Axz%3A139%26baseClass%3DilExerciseHandlerGUI&amp;app=com.apple.Safari&amp;css=3&amp;js=1&amp;rel=1&amp;rji=1&amp;sbe=1"></script>
<script type="text/javascript" nonce="19436f72e03846cb91b32bc5bbe" src="//local.adguard.org?ts=1748460873584&amp;name=AdGuard%20Extra&amp;type=user-script"></script><link rel="stylesheet" href="style.css">
</head>

<body>
<div>
    <img src="umg-zolty.png">
    <span class="headName">Uniwersytet Morski w Gdyni</span>
    <img src="budynekUMG.jpg">
</div>

<h2>Formularz rejestracyjny</h2>
<form>
    <label for="lname">Nazwisko</label>
    <input type="text" id="lname" name="lname">
    <label for="name">Imię</label>
    <input type="text" id="name" name="name"><br>
    <label for="mail">Adres e-mail</label>
    <input type="text" id="mail" name="mail">
</form>

<br>

<span>Województwo</span>
<select>
    <option value="opcja1">pomorskie</option>
    <option value="opcja2">mazowieckie</option>
</select><br><br>


<span>Wydział:</span>
<form>
    <input type="checkbox" id="vehicle1" name="vehicle1" value="Bike">
    <label for="vehicle1">Elektryczny</label><br>
    <input type="checkbox" id="vehicle2" name="vehicle2" value="Car">
    <label for="vehicle2">Mechaniczny</label><br>
    <input type="checkbox" id="vehicle3" name="vehicle3" value="Boat">
    <label for="vehicle3">Nawigacyjny</label><br>
    <input type="checkbox" id="vehicle4" name="vehicle4" value="Boat">
    <label for="vehicle4">Przedsiębiorczości i towaroznawstwa</label><br>
</form><br>

<span>Chcę otrzymywać:</span>
<input type="checkbox" name="check" class="chose" onclick="onlyOne(this)">
<span>tylko informacje na temat rekrutacji</span>
<input type="checkbox" name="check" class="chose" onclick="onlyOne(this)">
<span>wszystkie informacje</span><br><br>

<span>Uwagi/komentarze</span><br>
<textarea> </textarea><br><br>
<input type="submit" value="Wyśli"><br><br>


<a href="index.html">Powrót do strony głównej</a><br>

<script>
    function onlyOne(checkbox) {
    var checkboxes = document.getElementsByName(checkbox.name)
    checkboxes.forEach((item) => {
        if (item !== checkbox) item.checked = false
    })
}
</script>
</body>
</html>




```

</details>

<details>
<summary><strong>CSS</strong></summary>

```css
.headName {
    font-weight: bold;
    font-size: 28px;
}

.history tr, .history td {
    border: 1px solid;
    min-width: 80px;
    padding: 5px;
}

textarea {
    min-width: 300px;
    min-height: 100px;
}

#mail {
    min-width: 365px;
}

.chose {
    width:15px;
  height: 15px;
  border-radius: 50%;
  vertical-align: middle;
  border: 1px solid black;
  appearance: none;
  cursor: pointer;
}
.chose:checked {
    appearance: auto;
    clip-path: circle(50% at 50% 50%);
    background-color: blue;
  }
```

</details>

### 🖼️ Podgląd

<img width="1171" alt="Screenshot 2025-05-28 at 21 45 22" src="https://github.com/user-attachments/assets/a1c89b53-d8e7-4b66-bd9d-417dc41c2ff3" />

---

## Lab 2

### 📄 Opis  
Było podane prosta strona html, trzeba było podłączyć plik css i zrobić prosty style.
jako ostatnie zadanie trzebo było zmienić html i css i dodać nowy podpunkt z bannerami i zrobić, że po kliknieću po nim otwierała się nowa karta z podanym linkiem

### 🔧 Technologie  
`HTML`, `CSS`

### 💻 Kod

<details>
<summary><strong>HTML</strong></summary>

```html
<!DOCTYPE html>
<html lang="pl">
<head>
  <meta charset="utf-8">
  <meta name="Description" content=" Bookrossing - propagowanie idei czytania książek poprzez ich uwalnianie. Losy książek można sledzić.">
  <meta name="Keywords" content="book, bookcrossing, książka, uwalnianie, ruch uwalniania książek">
  <meta name="Author" content="ER">
  <meta name="Generator" content="kED">
	
	<title>BookCrossing</title>
  
  <script type="text/javascript" nonce="19436f72e03846cb91b32bc5bbe" src="//local.adguard.org?ts=1748460873584&amp;type=content-script&amp;dmn=ilias.umg.edu.pl&amp;url=https%3A%2F%2Filias.umg.edu.pl%2Filias.php%3Fref_id%3D114340%26ass_id%3D12162%26_table_nav%3Dfiletitle%3Aasc%3A0%26delivered%3D186743%26cmd%3Ddownload%26cmdClass%3Dilexsubmissionfilegui%26cmdNode%3Dxu%3A131%3Axz%3A139%26baseClass%3DilExerciseHandlerGUI&amp;app=com.apple.Safari&amp;css=3&amp;js=1&amp;rel=1&amp;rji=1&amp;sbe=1"></script>
<script type="text/javascript" nonce="19436f72e03846cb91b32bc5bbe" src="//local.adguard.org?ts=1748460873584&amp;name=AdGuard%20Extra&amp;type=user-script"></script><link rel="stylesheet" href="#" type="text/css">
  <link rel="stylesheet" href="bcstyl.css">
</head>

<body>
 
<div id="tytul"><h1><img src="bclogo.jpg" alt="logo"> BookCrossing - podaj książkę</h1></div>

<!--wstęp -->

<div>
<h2>Idea bookcrossingu</h2>

<p>
BookCrossing to ruch, którego celem jest propagowanie idei czytania książek. Polega na
<q>uwalnianiu</q>  książek tak aby mogła je znaleźć inna osoba, a następnie po przeczytaniu ponownie <q>uwolnić</q>.</p>
<p>
Ruch powstał w Stanach Zjednoczonych
<span>(<a href="http://www.bookcrossing.com">www.bookcrossing.com</a>)</span>,
natomiast obecnie rozwija się w wielu krajach, również w Polsce <span>(zobacz strony
<a href="http://www.bookcrossing.pl">www.bookcrossing.pl</a>,
<a href="http://www2.gazeta.pl/ksiazki/"> www2.gazeta.pl/ksiazki</a>)</span>.
</p>
</div>


<!-- część 1 -->

<div>
<h2>Zasady działania</h2>
<h3>Uczestnictwo</h3>

<p>Aby wziąć udział w akcji należy:</p>

<ul>
<li>Zarejestrować się w bazie uczestników.</li>
<li>Zarejestrować książkę w bazie książek.</li>
<li>Oznakować książkę naklejką z numerem.</li>
<li>Uwolnić książkę.</li>
</ul>


<p>
Dzięki rejestracji możemy śledzić losy książki i wiedzieć, kto ma naszą książkę, co o niej sądzi i
co z nią zrobił.
</p>

<h3>Sposoby uwalniania książek</h3>

<h4>Sposób pierwszy</h4>

<p>
Książkę zostawiamy w parku, na ławce, w pociągu, tramwaju, autobusie lub gdziekolwiek indziej,
pamiętając, że powinno to być miejsce uczęszczane, a nie kompletne odludzie. I czekamy, aż pojawi
się pierwszy wpis o <q>naszej</q> książce, czyli pierwszy znak, że ktoś ją odnalazł i zgłosił ten
fakt na stronie BookCrossing Polska. Będziemy o tym wiedzieć na pewno, bo system wyśle do nas maila
z informacją, że książka <q>żyje</q> i <q>się znalazła</q>.
</p>

<h4>Sposób drugi</h4>
<p>
Książkę uwalniamy wśród przyjaciół, znajomych i współpracowników. Postępujemy tak, jak w przypadku
pierwszym, tyle że książki nie porzucamy na pastwę przypadkowego przechodnia, lecz wręczamy osobie
znanej, która wyraża chęć jej przeczytania. Możemy zaraz po wręczeniu książki dokonać wpisu, komu ją
daliśmy i kiedy - i wtedy ta osoba będzie się wstydzić, jeśli po przeczytaniu nie uwolni książki w
jeden z trzech wymienianych tu sposobów.
</p>

<h4>Sposób trzeci</h4>
<p>
Trzecim fundamentem są Oficjalne Strefy BookCrossing, czyli półki, skrzynie, strefy czy po prostu
miejsca znane pozostałym uczestnikom. Uwalniając książkę dokonujemy stosownego wpisu w bazie
informacji, co zdecydowanie ułatwia pozostałym czytelnikom "polowanie" na upatrzone pozycje.
</p>

<p>
Wkażdym z trzech przypadków podstawą jest zarejestrowanie książki na <a href="http://www.bookcrossing.pl">
www.bookcrossing.pl</a> w celu uzyskania numeru BIP, dokładne opisanie książki, czyli wpisanie
przynajmniej numeru i adresu strony <span>(albo przyklejenie specjalnej karteczki,
którą można wydrukować w trakcie rejestracji)</span>.
</p>
</div>


<!-- część 2 -->
<div>
<h2>Historia <q>BookCrossingu</q></h2>

<img src="bcksiazki.jpg" alt="książki">
<p>
BookCrossing powstał w Stanach Zjednoczonych w marcu 2001 roku. Ron Hornbaker, zajmujący się na co
dzień wdrażaniem projektów internetowych, postanowił stworzyć unikalną, jedyną w swoim rodzaju
społeczność internetową, powodującą przyjemne uczucia.
</p>
<p>
Pomysł przyszedł mu do głowy, gdy razem z żoną Kaori podziwiali PhotoTag.org i WheresGeorge.com
<span>(obydwa serwisy oparte są na pomyśle śledzenia czegoś w internecie: pierwszy dotyczy zdjęć,
drugi śledzi George'a czyli pieniądze, jaką drogę przebędzie <q>twój</q> banknot? - identyfikacja
odbywa się na podstawie nr seryjnego)</span>. Idea śledzenia zainspirowała Rona do stworzenia
bookcrossingu. Do projektu podszedł z wielkim entuzjazmem i rozpoczął prace natychmiast następnego
dnia po wielkim olśnieniu. Jego żona wymyśliła logo, a on zajął się programowaniem po tym jak
otrzymał pełne poparcie ze strony partnerów z pracy.
</p>
<p>
Przez pierwszy okres BC miało około 100 hitów na miesiąc. Wszystko zmieniło się w marcu 2002, kiedy
opublikowano artykuł w Book Magazine. Po tej publikacji idea zaczęła się bardzo szybko
rozprzestrzeniać i zaowocowała niezliczonymi publikacjami w prasie, programami radiowymi i
telewizyjnymi, stając się <q>the most popular reading group on the web</q> <span>(najbardziej
popularną
czytającą grupą {społecznością} w sieci)</span>.
BookCrossing pozwala dzielić się książkami i śledzić ich drogę. BookCrossing ma za zadanie śledzić
uwolnione książki. Jednak, co ważniejsze BookCrossing pozwala zawiązywać znajomości - liczy w tej
chwili 155 858 członków <span>(a liczba członków rośnie z godziny na godzinę)</span>. Członkowie
BookCrossing to ludzie, którzy czytają książki, kochają książki i chcą się nimi dzielić z innymi.
</p>
</div>


<!-- część 3 -->
<div>
<h2>Historia <q>BookCrossingu</q> w Polsce</h2>
<p>Idea bookcrossingu w Polsce pojawiła się w październiku 2003 roku. Równolegle uruchomiono dwa polskie portale boockrossingowe: pierwszy <span>(www.bookcrossing.pl)</span> z inicjatywy Macieja Ślużyńskiego i Lechosława Gawrońskiego i drugi <span>(www.gazeta.pl/podajksiazke)</span> - za sprawą Tomasza Brzozowskiego wspieranego przez Gazetę Wyborczą.</p>

<p>Od roku 2004 bookcrosserzy w Polsce obchodzą Ogólnopolskie <q>Święto Wolnych Książek</q>, organizując marsze i happeningi. Pierwsze Święto Wolnych Książek odbyło się 6 kwietnia 2004 roku, w dniu urodzin jednego z inicjatorów bookcrossingu w Polsce. W późniejszych latach data ta została zmieniona pod wpływem sugestii nauczycieli.</p>

<p>8 kwietnia 2013 roku z inicjatywy Zrzeszenia Studentów Polskich akcja bookcrossingowa ruszyła na Uniwersytecie Warszawskim. W pierwszym dniu akcji udało się uwolnić 200 książek pozyskanych dzięki uczynności instytucji kulturalno-oświatowych.</p>

<p>Od roku 2004 mamy w Polsce Ogólnopolskie Święto Wolnych Książek. Obecnie obchodzi się je 12 czerwca. W tym dniu przeprowadzana jest ogólnopolska akcja uwalniania książek, połączona z przemarszami młodzieży. Organizowane są również happeningi, festyny, spotkania z autorami, wydawcami, debaty o książkach i literaturze, wystawy, konkursy czy plenerowe czytanie.</p>

<p>Funkcję ogólnopolskiego koordynatora bookcrossingu pełni od 2003 r. Jolanta Niwińska, nauczyciel bibliotekarz.</p>

</div>


<!-- część 4 -->
<div>
<h2>Przykłady <q>uwolnionych książek</q> - <a href="http://www.bookcrossing.pl">bookcrossing</a></h2>

<table id="przyklad">
<tr><td>Tytuł</td> <td>Autor</td> <td>Uwolniona</td></tr>
<tr><td>Błękitny Zamek</td> <td>Lucy Maud Montgomery</td> <td>2019-10-27</td></tr>
<tr><td>Stara Ziemia</td> <td>Jerzy Żuławski</td> <td>2019-10-27</td> </tr>
<tr><td>Zwycięzca</td> <td>Jerzy Żuławski</td> <td>2019-10-29</td> </tr>
<tr><td>Wieża zakładników</td> <td>Alistair MacLean</td><td> 2019-10-30</td> </tr>
<tr><td>Cudowny czwartek</td><td> John Steinbeck</td><td> 2019-10-31</td> </tr>
<tr><td>Klopoty rodu Pożyczalskich</td><td>Mary Norton</td><td> 2019-11-06</td> </tr>
<tr><td>Złoty faraon</td><td>Karl Bruckner</td><td> 2019-11-06</td> </tr>
</table>
</div>

<!-- część 5 -->

<div>
<h2>Przykład formularza do rejestrowania uczestników i książek</h2>

<form action="x">
<fieldset><legend>Dane uczestnika</legend>
<label>Podaj swoje imię <input type="text"></label>
<label> i nazwisko <input type="text"></label><br>
<label>Podaj pseudonim, którego chcesz używać <input type="text"></label>
</fieldset>
</form>
<form action="x">
<fieldset><legend>Dane uwalnianej książki</legend>
<label>Tytuł: <input type="text" size="40"></label><br>
<label>Autor: <input type="text" size="40"></label><br>
<label>Data uwolnienia: <input type="text"></label>
</fieldset>
</form>
</div>

<!-- część 1 -->
<h2>Akcje bookcrossingu </h2>

<a target="_blank" href="https://www.uwalniamyksiazki.pl/"><img src="link1.png" alt="logo"></a><br>
<a target="_blank" href="https://zsriojagarzewo.pl/index.php/98-aktualnosci/844-akcja-uwolnij-ksiazke-bookcrossing"><img src="link2.png" alt="logo"></a><br>
<a target="_blank" href="https://biblioteka.pl/temat/Bookcrossing/Artykuly"><img src="link3.png" alt="logo"></a><br>
<a target="_blank" href="https://www.sp3zawiercie.pl/kategorie/akcja-uwalniania-ksiazek-bookcrossing"><img src="link4.png" alt="logo"></a><br>
<a target="_blank" href="http://zsat.linuxpl.eu/biblioteka/boockcrossing/"><img src="link5.png" alt="logo"></a><br>

</body>
</html>


```

</details>

<details>
<summary><strong>CSS</strong></summary>

```css
body {
    background-color:#f0e766;
}

h2 {   
    background: #4dbc49;
    border-bottom: 3px dotted #f8c3cd;
    border-left: 3px dotted #f8c3cd;
    font-size: 32px;
}

h3 {   
    background: #0fffa5;
    border-bottom: 3px dotted #f8e6d2;
    border-right: 3px dotted #f8e6d2;
}

form {
    background: #84867a;
    border: orange, solid, 2px;
}

h1 {
    color: #12437f;
    font-size: 42px;
    text-align: center;
}

#tytul {
    border: #291107, dashed, 4px;
}

p {
    font-family: Arial, Helvetica, sans-serif;
    color: #857770;
}

tr:first-child td {
    font-family: Georgia, serif;
    font-weight: bold;
    color: #291107;
}

ul {
    list-style: url('diam.png');
}

a img {
    height: 100px;
    width: 250px;
  object-fit: cover;
}
a img:hover {
    -webkit-filter: brightness(70%);
}
```

</details>

### 🖼️ Podgląd

<img width="1626" alt="Screenshot 2025-05-28 at 21 52 38" src="https://github.com/user-attachments/assets/b7cfc90e-4251-4c23-a8f9-bdb6f067526f" />

---

## Lab 3

### 📄 Opis  
W ramach laboratorium stworzyliśmy prostą stronę internetową o dowolnej tematyce. Strona zawierała podstawowy layout z wykorzystaniem HTML i CSS, w tym: nagłówek (header), pasek nawigacyjny (nav), główną część strony (main) oraz stopkę (footer). Celem ćwiczenia było opanowanie struktury dokumentu HTML oraz zastosowanie CSS do rozmieszczenia i stylizacji elementów.

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
    <img id="header-img" src="https://b2ccdn.coraltravel.pl/content/banner/desktop/bannerslide_12032025134349.jpg" alt="Podróże - baner">
    
    <header>
        <h1>Twoja Przygoda – Odkryj Świat z Nami!</h1>
        <nav>
            <ul>
                <li><a href="#home">Strona główna</a></li>
                <li><a href="#about">O nas</a></li>
                <li><a href="#destinations">Najlepsze kierunki podróży</a></li>
                <li><a href="#tips">Porady podróżnicze</a></li>
                <li><a href="#contact">Kontakt</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section id="home">
            <h2>Witaj na naszej stronie podróżniczej!</h2>
            <p>Podróże to nie tylko przemieszczanie się – to styl życia. Odkryj z nami najpiękniejsze miejsca na świecie!</p>
        </section>

        <section id="about">
            <h2>O nas</h2>
            <p>Podróże to nasza pasja! Jesteśmy zespołem miłośników odkrywania świata, którzy chcą dzielić się z Tobą najlepszymi miejscami, poradami i inspiracjami. Dołącz do naszej społeczności i zacznij swoją przygodę!</p>
        </section>

        <section id="destinations">
            <h2>Najlepsze kierunki podróży</h2>
            <article>
                <h3>Bali – Rajska wyspa pełna magii</h3>
                <p>Odkryj piękne plaże, tropikalne dżungle i kulturę Bali. Sprawdź najlepsze miejsca do odwiedzenia!</p>
            </article>
            <article>
                <h3>Paryż – Miasto Miłości i Sztuki</h3>
                <p>Wieża Eiffla, Luwr, kawiarnie i romantyczna atmosfera – zobacz, dlaczego Paryż zachwyca turystów!</p>
            </article>
            <article>
                <h3>Islandia – Kraina lodu i ognia</h3>
                <p>Gorące źródła, lodowce i zorza polarna – Islandia to miejsce, które musisz zobaczyć na własne oczy!</p>
            </article>
        </section>

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
        </section>

        <section id="contact">
            <h2>Kontakt</h2>
            <p>Masz pytania? Skontaktuj się z nami! Chętnie pomożemy w zaplanowaniu Twojej wymarzonej podróży.</p>
        </section>
    </main>

    <footer>
        <p>© 2025 Twoja Przygoda. Wszystkie prawa zastrzeżone.</p>
    </footer>

    <script>
        document.addEventListener("DOMContentLoaded", function () {
            const navLinks = document.querySelectorAll("nav ul li a");

            navLinks.forEach(link => {
                link.addEventListener("click", function (e) {
                    e.preventDefault();
                    const targetId = this.getAttribute("href").substring(1);
                    const targetSection = document.getElementById(targetId);

                    if (targetSection) {
                        window.scrollTo({
                            top: targetSection.offsetTop - 50,
                            behavior: "smooth"
                        });
                    }
                });
            });
        });
    </script>

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
    background-color: #e0f7fa; /* Jasny błękit */
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

nav ul {
    list-style: none;
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 15px;
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
    transition: background 0.3s, transform 0.2s;
    display: inline-block;
}

nav ul li a:hover {
    background: #fb8c00;
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
    background: #fff3e0; /* Kolor piasku */
    border-radius: 8px;
    box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.1);
    text-align: center;
}

section h2 {
    font-size: 26px;
    margin-bottom: 15px;
    color: #ff7043; /* Ciepły pomarańczowy */
    border-bottom: 3px solid #ff7043;
    display: inline-block;
    padding-bottom: 5px;
}

article {
    background: #ffebee; /* Jasny różowy jak zachód słońca */
    padding: 20px;
    margin-bottom: 15px;
    border-radius: 8px;
    width: 100%;
    text-align: left;
    transition: transform 0.2s;
}

article:hover {
    transform: translateY(-5px);
}

article h3 {
    color: #d32f2f; /* Czerwony jak zachód słońca */
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

<img width="144" alt="Screenshot 2025-05-28 at 21 55 43" src="https://github.com/user-attachments/assets/64a86aa8-855a-42ac-aa95-3fb9cfa8d6b5" />

<img width="1438" alt="Screenshot 2025-05-28 at 21 56 00" src="https://github.com/user-attachments/assets/305b8e36-0122-4a4d-bff4-f7f1659e6984" />

---

## Lab 4

### 📄 Opis  
Na podstawie przykładów z zajęć (1–7) zmodyfikowaliśmy layout z poprzedniego laboratorium. Celem było przetestowanie różnych metod pozycjonowania elementów na stronie. Wykorzystano techniki takie jak:

- pozycjonowanie absolutne (position: absolute)

- pływające elementy (float)

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
                <li><a href="#home">Strona główna</a></li>
                <li><a href="#about">O nas</a></li>
                <li><a href="#destinations">Najlepsze kierunki podróży</a></li>
                <li><a href="#tips">Porady podróżnicze</a></li>
                <li><a href="#contact">Kontakt</a></li>
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
        </section>

        <section id="contact">
            <h2>Kontakt</h2>
            <p>Masz pytania? Skontaktuj się z nami! Chętnie pomożemy w zaplanowaniu Twojej wymarzonej podróży.</p>
        </section>
    </main>

    <footer>
        <p>© 2025 Twoja Przygoda. Wszystkie prawa zastrzeżone.</p>
    </footer>

    <script>
        document.addEventListener("DOMContentLoaded", function () {
            const navLinks = document.querySelectorAll("nav ul li a");

            navLinks.forEach(link => {
                link.addEventListener("click", function (e) {
                    e.preventDefault();
                    const targetId = this.getAttribute("href").substring(1);
                    const targetSection = document.getElementById(targetId);

                    if (targetSection) {
                        window.scrollTo({
                            top: targetSection.offsetTop - 50,
                            behavior: "smooth"
                        });
                    }
                });
            });
        });
    </script>

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
    height: 125px;
    max-width: 100%;
    box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.2);
}

header h1 {
    font-size: 28px;
    margin-bottom: 10px;
}

nav ul {
    list-style: none;
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 15px;
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
    transition: background 0.3s, transform 0.2s;
    display: inline-block;
}

nav ul li a:hover {
    background: #fb8c00;
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

<img width="1017" alt="Screenshot 2025-05-28 at 22 17 14" src="https://github.com/user-attachments/assets/c74506a2-a965-49db-b284-dc91f8598de5" />

---

## Lab 5

### 📄 Opis  
Celem zadania było zaprojektowanie layoutu strony internetowej zgodnie z dokładnymi wytycznymi dotyczącymi rozmiarów, kolorów i układu bloków. Kluczowym wymaganiem było poprawne rozmieszczenie elementów za pomocą CSS oraz ich wyśrodkowanie w pionie i poziomie. Struktura strony miała zostać zbudowana z bloków oznaczonych jako A1–A4 i B1–B2, a dodatkowo należało sformatować nagłówki (h1, h3) oraz odpowiednio wyrównać listę uporządkowaną i nieuporządkowaną. Zadanie miało na celu sprawdzenie znajomości podstawowego pozycjonowania, pracy z box model oraz umiejętności odwzorowania układu graficznego w kodzie HTML i CSS.

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
    <link rel="stylesheet" href="css/style.css">
</head>
<body>
    <header>
        <h1>KOLOKWIUM</h1>
    </header>
    <main>
        <aside>
            <ol start="10">
                <li>opcja 1</li>
                <li>opcja 2</li>
                <li>opcja 3</li>
                <li>opcja 4</li>
                <li>opcja 5</li>
            </ol> 
        </aside>
        <content>
            <section id="B1">

            </section>
            <section id="B2">
                
            </section>
        </content>
        
        <section id="A1">
            <ul type="disc">
                <li> opcja 1</li>
                <li> opcja 2</li>
                <li> opcja 3</li>
            </ul>
        </section>
        <footer id="A4">
            <h3>mikanovich-03.04.2025</h3>
        </footer>
    </main>
</body>

</html>
```

</details>

<details>
<summary><strong>CSS</strong></summary>

```css
body {
    flex-direction: column;
    display: flex;
    justify-content: center;
    align-items: center;
    width: 1000px;
    margin:0 auto;
}

header{
    width:700px; 
    height:50px;
    overflow: hidden; 
    background-color:lightblue;
    justify-content: center;
    align-items: center;
    display: flex;
}

h1{
    text-align: center;
    color: white;
}

aside{
    width:200px; 
    height:500px;
    position:relative;
    top:0px;
    right:100px;
    background-color:lightblue;
    justify-content: center;
    align-items: center;
    display: flex;
}

aside ol {
    list-style-type: upper-roman;
}

section#A1{
    width:200px; 
    height:200px;
    background-color:lightblue;
    position:absolute;
    top:350px;
    left:1190px;
    justify-content: center;
    align-items: center;
    display: flex;
}

footer{
    width:900px; 
    height:50px;
    background-color:lightblue;
    position:relative;
    top:0px;
    left:100px;
    align-items: center;
    justify-content: flex-end;
    display: flex;
}

h3{
    text-align: center;
    position:relative;
    right: 20px;
}

content {
    position: absolute;
    top: 50px;
    left: 490px;
    display: flex;
}

section#B1{
    margin: 10px;
    width:200px; 
    height:210px;
    background-color:yellow;
}

section#B2{
    margin: 10px;
    width:470px; 
    height:210px;
    background-color:yellow;
}
```

</details>

### 🖼️ Podgląd

<img width="1237" alt="Screenshot 2025-04-03 at 09 52 01" src="https://github.com/user-attachments/assets/47f6f2ec-21fe-401b-b1f9-d27d879f898f" />



➡️ [Przejdź do kolejnej części: documentation2.md](documentation2.md)

