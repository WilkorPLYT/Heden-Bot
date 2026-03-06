# 🤝 Przewodnik Wkładu (Contributing Guide)

Dziękuję za zainteresowanie wkładem w projekt **HEDEN Cargo Bot**! 

## 📋 Spis Treści

- [Jak Zacząć](#-jak-zacząć)
- [Proces Pull Request](#-proces-pull-request)
- [Wytyczne Kodowania](#-wytyczne-kodowania)
- [Raportowanie Błędów](#-raportowanie-błędów)

---

## 🚀 Jak Zacząć

### 1. Fork Repozytorium

Kliknij przycisk **Fork** w górnym prawym rogu

### 2. Sklonuj Do Lokalnego Repo

```bash
git clone https://github.com/YOUR_USERNAME/HedenCargoWeb.git
cd HedenCargoWeb
```

### 3. Stwórz Nową Gałąź (Branch)

```bash
git checkout -b feature/twoja-nowa-funkcja
# lub
git checkout -b bugfix/napraw-tego-bledy
```

Nazwy gałęzi:
- `feature/nazwa-funkcji` - dla nowych funkcji
- `bugfix/nazwa-bledu` - dla napraw
- `docs/nazwa-zmiany` - dla dokumentacji

### 4. Zainstaluj Zależności

```bash
npm install
```

### 5. Utwórz `.env.local` Dla Testowania

```bash
cp .env.example .env.local
# Edytuj z testowymi danymi
```

---

## 📤 Proces Pull Request

### Commitowanie

Używaj jasnych commitów:

```bash
# ✅ Dobry commit
git commit -m "feat: dodaj system backupu MongoDB"
git commit -m "fix: napraw błąd przy zatwierdzaniu zleceń"

# ❌ Zły commit
git commit -m "fix stuff"
```

Prefiks commitów:
- `feat:` - Nowa funkcja
- `fix:` - Naprawienie błędu
- `docs:` - Zmiany w dokumentacji
- `refactor:` - Refactoring kodu

### Wypchnij & Utwórz PR

```bash
git push origin feature/twoja-funkcja
```

Na GitHub'ie kliknij "Compare & pull request"

---

## 💻 Wytyczne Kodowania

### JavaScript

```javascript
// ✅ Preferuj const/let
const config = require('./config');

// ✅ Dokumentuj funkcje
/**
 * Wysyła embed do kanału Discord
 * @param {Channel} channel
 * @param {Object} embed
 */
async function sendEmbed(channel, embed) {
  return channel.send({ embeds: [embed] });
}

// ✅ Obsługuj błędy
try {
  await connectDatabase();
} catch (error) {
  logger.error('Błąd:', error);
}
```

---

Dziękuję za wkład! 🚀
