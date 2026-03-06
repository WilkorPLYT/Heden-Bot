# ❓ Frequently Asked Questions (FAQ)

## 🚀 Instalacja

### Jak zainstalować bota?

```bash
git clone https://github.com/WilkorPLYT/HedenCargoWeb.git
cd HedenCargoWeb
npm install
cp .env.example .env
# Edytuj .env
npm start
```

### Jak podłączyć Discord Token?

1. https://discord.com/developers/applications
2. Utwórz nową aplikację
3. Bot → Copy Token
4. Wklej do `.env` jako `DISCORD_TOKEN`

### Jak skonfigurować MongoDB?

**Lokalnie:**
```
MONGODB_URI=mongodb://localhost:27017/hedencargo
```

**Atlas (Cloud):**
```
MONGODB_URI=mongodb+srv://user:password@cluster.mongodb.net/hedencargo
```

---

## 🛠️ Troubleshooting

### Bot się nie startuje

```bash
# Sprawdź Node.js
node --version  # Powinna być 18+

# Zainstaluj zależności
npm install

# Sprawdź .env
cat .env
```

### MongoDB connection error

```bash
# Sprawdź czy MongoDB działa
mongosh

# Jeśli Atlas - sprawdzlogi IP whitelist
```

---

## 📞 Pomoc

| Developer | Discord | GitHub |
|-----------|---------|--------|
| **𝓓𝓻𝓦𝓲𝓵𝓴𝓸𝓻** | [𝓓𝓻𝓦𝓲𝓵𝓴𝓸𝓻](https://discord.com/users/446740090757316608) | [@WilkorPLYT](https://github.com/WilkorPLYT) |
| **daniek.** | [daniek.](https://discord.com/users/640502766959329282) | [@daniekdan](https://github.com/daniekdan) |

---

Nie znalazłeś odpowiedzi? Otwórz issue! 💬
