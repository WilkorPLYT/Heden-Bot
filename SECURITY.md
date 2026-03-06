# 🔒 Polityka Bezpieczeństwa

## Raportowanie Luk w Bezpieczeństwa

Jeśli odkryjesz lukę w bezpieczeństwie, **nie otwieraj publicznego issue**.

Skontaktuj się prywatnie:

| Developer | Discord | GitHub |
|-----------|---------|--------|
| **𝓓𝓻𝓦𝓲𝓵𝓴𝓸𝓻** | [𝓓𝓻𝓦𝓲𝓵𝓴𝓸𝓻](https://discord.com/users/446740090757316608) | [@WilkorPLYT](https://github.com/WilkorPLYT) |
| **daniek.** | [daniek.](https://discord.com/users/640502766959329282) | [@daniekdan](https://github.com/daniekdan) |

## Best Practices

1. **Nigdy nie commituj `.env` z sekretami**
2. **Używaj zmiennych środowiskowych** dla tokenów
3. **Weryfikuj dane od użytkowników**
4. **Loguj bezpiecznie** (bez haseł/tokenów)

### Bezpieczeństwo Token Discord

⚠️ **NIGDY nie udostępniaj:**
- `DISCORD_TOKEN`
- `MONGODB_URI` z hasłem

**JEŚLI token wyciekł:**
1. Natychmiast regeneruj token w [Developer Portal](https://discord.com/developers/applications)
2. Zaktualizuj `.env`
3. Restartuj bota
4. Sprawdź logi

---

Dziękuję za pomoc w utrzymaniu bezpieczeństwa! 🔒
