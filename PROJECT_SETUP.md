# 🚀 Przewodnik Konfiguracji Projektu

Kompletny poradnik do uruchomienia HEDEN Cargo Bot lokalnie.

## 🔧 Wymagania

- **Node.js** 18.0.0+
- **npm** 9.0.0+ lub **yarn**
- **MongoDB** 4.4+
- **Git**

---

## 📦 Instalacja Lokalna

### Krok 1: Klonuj Repozytorium

```bash
git clone https://github.com/WilkorPLYT/HedenCargoWeb.git
cd HedenCargoWeb
```

### Krok 2: Zainstaluj Zależności

```bash
npm install
```

### Krok 3: Utwórz `.env`

```bash
cp .env.example .env
```

Edytuj `.env` i dodaj swoje tokeny (patrz poniżej)

### Krok 4: Zainstaluj MongoDB

**Opcja A: Lokalnie**
```bash
# Pobierz z https://www.mongodb.com/try/download/community
# Lub brew install mongodb-community (macOS)
```

**Opcja B: MongoDB Atlas (Cloud)**
1. Przejdź na https://www.mongodb.com/cloud/atlas
2. Utwórz darmowy cluster
3. Skopiuj connection string do `.env`

### Krok 5: Discord Token

1. Przejdź na [Discord Developer Portal](https://discord.com/developers/applications)
2. Utwórz nową aplikację
3. Przejdź na zakładkę "Bot" i skopiuj token
4. Wklej do `.env`:

```env
DISCORD_TOKEN=your_bot_token_here
APPLICATION_ID=your_app_id_here
GUILD_ID=your_server_id_here
OWNER_ID=your_user_id_here
MONGODB_URI=mongodb+srv://user:password@cluster.mongodb.net/hedencargo
```

---

## ▶️ Uruchamianie

### Development (z auto-reload)
```bash
npm run dev
```

### Produkcja
```bash
npm start
```

---

Dla pełnego poradnika zobacz [README.md](README.md)
