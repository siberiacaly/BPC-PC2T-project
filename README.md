# Projekt do předmětu BPC-PC2T

## Zadání projektu

Cílem semestrální práce bylo vytvořit **objektově orientovanou aplikaci** v jazyce Java pro správu **filmové databáze**.
Systém rozlišuje dva typy snímků: **hrané filmy** (s herci) a **animované filmy** (s animátory a doporučeným věkem).
Aplikace umožňuje komplexní manipulaci s daty, vyhledávání, filtrování a zajišťuje **trvalé uložení dat** pomocí SQL databáze.

---

## 1. Struktura a správa filmů

Jádrem aplikace je hierarchie tříd reprezentující různé druhy filmů. Uživatel může dynamicky spravovat seznam titulů v paměti.

**Hlavní funkce správy:**
- **Přidání a editace:** Vkládání nových filmů s atributy (název, režisér, rok, herci/animátoři).
- **Rozlišení typů:**
    - *Hraný film:* Hodnocení 1–5 hvězdiček.
    - *Animovaný film:* Hodnocení 1–10 bodů + doporučený věk.
- **Hodnocení:** Uživatel může přidávat bodové i slovní hodnocení k existujícím záznamům.

---

## 2. Pokročilá práce s daty a perzistence

Projekt implementuje několik úrovní ukládání a načítání dat, aby informace zůstaly zachovány i po ukončení programu.

**Způsoby uložení:**
- **SQL Databáze:** Při spuštění se data automaticky načtou z databáze a při ukončení se do ní změny uloží (automatická synchronizace).
- **Export/Import do souboru:** Možnost manuálně uložit/načíst informace o konkrétním filmu do textového souboru.

**Analytické funkce:**
- 🔍 **Vyhledávání:** Detailní výpis informací o filmu včetně seřazených hodnocení.
- 👥 **Analýza tvůrců:**
    - Výpis herců/animátorů podílejících se na více filmech.
    - Filtrování všech filmů podle konkrétního tvůrce.

---

## Odkaz na kód

- [💾 Zdrojové kódy (ProjectFilms)](./ProjectFilms)

---

## Shrnutí funkcionality

- ✅ Objektový návrh (dědičnost, polymorfismus)
- ✅ CRUD operace (Create, Read, Update, Delete) nad filmy
- ✅ Rozlišení logiky pro hrané a animované filmy
- ✅ Pokročilé vyhledávání podle herců a animátorů
- ✅ Práce se soubory (export/import jednotlivých položek)
- ✅ Napojení na SQL databázi (automatické načítání a ukládání)

---

## Použité platformy a technologie

- Jazyk: **Java** (JDK 17+)
- Databáze: **SQL** (např. SQLite/MySQL přes JDBC)
- Rozhraní: **Konzolové UI**
- Koncepty: **OOP, Collections Framework, JDBC, File I/O**

---

> Projekt byl vypracován Tomášem Calábkem (ID: 237881) pro kurz **BPC-PC2T** (Počítače a programování 2) na VUT FEKT.
