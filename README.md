# 📝 jsonVerter

**jsonVerter** è un'applicazione desktop per Windows che consente di convertire file `.txt` in file `.json` strutturati, tramite un'interfaccia grafica semplice e intuitiva. Ogni riga del file `.txt` viene trasformata in un oggetto JSON, con supporto multilingua.

---

## 🚀 Caratteristiche principali

- Interfaccia grafica facile da usare
- Conversione automatica da `.txt` a `.json`
- Aggiunta automatica di ID per ogni elemento
- Supporto multilingua: lingua di origine + lingue di destinazione
- 100% offline, senza dipendenze esterne
- Controllo aggiornamenti integrato

---

## 🖥️ Requisiti

- Sistema operativo: **Windows**
- Non è richiesta alcuna installazione di Python o librerie esterne
- Applicazione completamente standalone (`.exe`)

---

## 📝 Formattazione del file .txt

Il file `.txt` deve contenere le frasi da convertire in JSON, **una per riga**.

### ✅ Esempio corretto:
```txt
content 1
content 2
content 3
```

Ogni riga rappresenta un contenuto da tradurre e inserire nel file JSON finale.

### ⚠️ Attenzione:
- **Non** lasciare righe vuote.
- **Non** usare virgolette o altri simboli speciali.
- **Non** separare frasi con virgole o punti e virgola nella stessa riga.

### 📌 Suggerimento:
Se vuoi dividere i contenuti in categorie, crea un file `.txt` per categoria.


## 🛠️ Come usare jsonVerter

1. Scarica il file `jsonVerter.exe`.
2. Esegui il programma con doppio clic (non serve installazione).
3. Nell'interfaccia:
   - 📂 Seleziona il file `.txt` di input.
   - 💾 Specifica il percorso per il file `.json` di output.
   - 🌐 Inserisci la **lingua di origine** (es. `it`).
   - 🌍 Inserisci le **lingue di traduzione**, separate da virgola (es. `en,fr`).
   - 🔄 Clicca su **Converti** per generare il file JSON.
4. 🔄 Usa il pulsante **Controlla aggiornamenti** per verificare se è disponibile una nuova versione.

---

## 📄 Formato JSON di output

```json
{
  "items": [
    { "id": 1, "content": "Prima riga del file" },
    { "id": 2, "content": "Seconda riga del file" }
  ],
  "source_lang": "it",
  "dest_langs": ["en", "fr"]
}
