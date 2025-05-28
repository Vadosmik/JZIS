
# 🧪 Dokumentacja laboratoriów

Zestawienie wykonanych laboratoriów z przedmiotu XYZ. Każdy wpis zawiera krótki opis, kod źródłowy oraz podgląd działania.

---

## 📋 Spis treści

- [Lab 1 — Prosty layout strony](#lab-1--prosty-layout-strony)
- [Lab 2 — Formularz logowania](#lab-2--formularz-logowania)
- [Lab 3 — Lista TODO w JavaScript](#lab-3--lista-todo-w-javascript)

---

## Lab 1 — Prosty layout strony

### 📄 Opis  
Celem było stworzenie prostego layoutu strony głównej przy użyciu HTML i CSS (Flexbox). Strona zawiera nagłówek, główną sekcję i stopkę.

### 🔧 Technologie  
`HTML`, `CSS`

### 💻 Kod

<details>
<summary><strong>HTML</strong></summary>

```html
<!DOCTYPE html>
<html lang="pl">
<head>
  <meta charset="UTF-8" />
  <title>Prosty Layout</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <header>
    <h1>Moja strona</h1>
  </header>
  <main>
    <p>To jest treść główna.</p>
  </main>
  <footer>
    <p>Stopka</p>
  </footer>
</body>
</html>
```

</details>

<details>
<summary><strong>CSS</strong></summary>

```css
body {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
  margin: 0;
  font-family: sans-serif;
}
header, footer {
  background-color: #333;
  color: white;
  padding: 1em;
  text-align: center;
}
main {
  flex: 1;
  padding: 2em;
}
```

</details>

### 🖼️ Podgląd

![Lab 1 Screenshot](./screenshots/lab1.png)

---

## Lab 2 — Formularz logowania

### 📄 Opis  
Stworzenie prostego formularza logowania z walidacją po stronie przeglądarki. Formularz sprawdza, czy pola zostały uzupełnione.

### 🔧 Technologie  
`HTML`, `CSS`, `JavaScript`

### 💻 Kod

<details>
<summary><strong>HTML</strong></summary>

```html
<form id="loginForm">
  <label for="username">Login:</label>
  <input type="text" id="username" required />

  <label for="password">Hasło:</label>
  <input type="password" id="password" required />

  <button type="submit">Zaloguj</button>
</form>
```

</details>

<details>
<summary><strong>CSS</strong></summary>

```css
form {
  max-width: 300px;
  margin: auto;
  padding: 1em;
  border: 1px solid #ccc;
  border-radius: 4px;
}
label, input {
  display: block;
  margin-bottom: 0.5em;
}
```

</details>

<details>
<summary><strong>JavaScript</strong></summary>

```js
document.getElementById('loginForm').addEventListener('submit', function(e) {
  e.preventDefault();
  const user = document.getElementById('username').value;
  const pass = document.getElementById('password').value;

  if (user && pass) {
    alert(`Witaj, ${user}!`);
  } else {
    alert("Uzupełnij wszystkie pola!");
  }
});
```

</details>

### 🖼️ Podgląd

![Lab 2 Screenshot](./screenshots/lab2.png)

---

## Lab 3 — Lista TODO w JavaScript

### 📄 Opis  
Prosta aplikacja typu TODO, umożliwiająca dodawanie oraz usuwanie zadań z listy. Użyto czystego JavaScriptu bez frameworków.

### 🔧 Technologie  
`HTML`, `CSS`, `JavaScript`

### 💻 Kod

<details>
<summary><strong>HTML</strong></summary>

```html
<h1>Lista zadań</h1>
<input type="text" id="taskInput" placeholder="Nowe zadanie" />
<button onclick="addTask()">Dodaj</button>
<ul id="taskList"></ul>
```

</details>

<details>
<summary><strong>CSS</strong></summary>

```css
body {
  font-family: sans-serif;
  text-align: center;
  padding: 2em;
}
input {
  padding: 0.5em;
}
button {
  margin-left: 0.5em;
}
ul {
  list-style: none;
  padding: 0;
}
li {
  margin: 0.5em 0;
  cursor: pointer;
}
```

</details>

<details>
<summary><strong>JavaScript</strong></summary>

```js
function addTask() {
  const input = document.getElementById("taskInput");
  const task = input.value.trim();
  if (task) {
    const li = document.createElement("li");
    li.textContent = task;
    li.onclick = () => li.remove();
    document.getElementById("taskList").appendChild(li);
    input.value = "";
  }
}
```

</details>

### 🖼️ Podgląd

![Lab 3 Screenshot](./screenshots/lab3.png)

---
