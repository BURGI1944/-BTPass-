# 🔐 $$BTPass$$ – Offline USB správca hesiel (.EXE, šifrovaný)

## 🧰 Čo je $$BTPass$$?

**$$BTPass$$** je bezpečný offline správca hesiel zabalený do jediného `.exe` súboru.  
Ukladá tvoje šifrované heslá **na USB kľúč** (alebo ľubovoľné iné úložisko), s použitím **AES-256-GCM šifrovania** a hlavného hesla.  
Žiadna inštalácia, žiadne závislosti, žiadne pripojenie k internetu – stačí spustiť EXE súbor.

---

## 💡 Hlavné funkcie

- 🔒 Ochrana Master heslom (AES-GCM + PBKDF2)
- 💾 Ukladanie a čítanie šifrovaných hesiel z USB
- 🔑 Generátory hesiel:
  - Klasické (nízka / stredná / vysoká zložitosť)
  - Nezmyselné (úplne náhodné)
  - Logické (na základe zadaného slova)
- ✏️ Pridávanie, zobrazenie a mazanie hesiel
- 🔐 Zmena Master hesla s prešifrovaním všetkých údajov
- 🧠 Kontrola integrity dát (detekcia manipulácie / zlé heslo)
- 🪟 Konzolové rozhranie (kompatibilné s Windows)

---

## 📁 Kam sa ukladajú tvoje dáta

Heslá sú uložené lokálne (na USB alebo inú cestu, ktorú si zvolíš):

<disk>:/PassAeSPassAeS/PassPass.json

Cesta sa zapamätá v súbore `config.json`, ktorý je uložený vedľa EXE.

---

## 🚀 Ako to používať

1. Spusť `$$BTPass$$.exe`
2. Pri prvom spustení ťa program vyzve na zadanie cesty k úložisku a nastavenie Master hesla
3. Vyber si možnosť z hlavného menu:
   - Zobraziť uložené heslá
   - Vygenerovať nové (klasické, nezmyselné, logické)
   - Pridať vlastné heslo
   - Vymazať záznam
   - Zmeniť Master heslo
4. Všetky dáta sú bezpečne šifrované tvojím Master heslom

> 💡 Nie je potrebné inštalovať Python ani nič iné. Je to prenosná `.exe` aplikácia.

---

## 🛡️ Bezpečnosť

- Šifrovanie AES-256-GCM
- Master heslo sa nikdy nikde neukladá
- Kľúč je odvodený pomocou PBKDF2 (so soľou a 160 000 iteráciami)
- Všetko beží **offline** – žiadny cloud, žiadne synchronizácie, žiadne riziko z internetu

---

## 👤 Autor

**BURGI**  
📅 Vytvorené v roku 2025  
📌 Vytvorené pomocou Python + PyInstaller (`--onefile`)

---

## ❗ Licencia

**Tento projekt je uzavretý (proprietárny) softvér.**  
Všetky práva vyhradené © 2025 BURGI.  
Kopírovanie, šírenie alebo úprava sú zakázané bez výslovného súhlasu.
