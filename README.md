# JZIS

# 📘 Dokumentacja laboratoriów

## ✅ Spis treści
1. [Lab 1 — Tytuł / temat](#lab-1---tytuł--temat)
2. [Lab 2 — Tytuł / temat](#lab-2---tytuł--temat)
3. [Lab 3 — Tytuł / temat](#lab-3---tytuł--temat)

---

## 🧪 Lab 1 — Tytuł / temat <a name="lab-1---tytuł--temat"></a>

### 📄 Opis  
Krótki opis tego, czego dotyczył lab.  
Np.  
> Celem było stworzenie prostego layoutu strony głównej z użyciem HTML i CSS, z wykorzystaniem Flexboxa.

---

### 🔧 Technologie  
`HTML`, `CSS`, `JavaScript` *(jeśli dotyczy)*

---

### 💻 Kod

<details>
<summary><strong>HTML</strong></summary>

```html
<!DOCTYPE html>
<html lang="pl">
<head>
  <meta charset="UTF-8" />
  <title>Moja Strona</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <header>
    <h1>Witaj!</h1>
  </header>
</body>
</html>
</details>
<details>
<summary><strong>CSS</strong></summary>
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
</details>
🖼️ Podgląd

Lab 2 — Formularz logowania

📄 Opis

Stworzenie prostego formularza logowania z walidacją po stronie przeglądarki. Formularz sprawdza, czy pola zostały uzupełnione.

🔧 Technologie

HTML, CSS, JavaScript

💻 Kod
