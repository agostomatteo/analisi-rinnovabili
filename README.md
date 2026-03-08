# ⚡ Analisi Energie Rinnovabili Italia (2021–2026)

Progetto personale di analisi dati sulla produzione di energia rinnovabile in Italia,
basato sui dati ufficiali di **Terna** (Gestore della Rete di Trasmissione Nazionale).

---

## 📁 Struttura del progetto

| Notebook | Descrizione |
|---|---|
| `Analisi_Rinnovabili.ipynb` | Pulizia e preparazione del dataset grezzo (dati orari → mensili) |
| `Analisi_per_Fonte.ipynb` | Analisi della produzione fonte per fonte (solare, eolico, idrico…) |
| `Analisi_Stagionale.ipynb` | Variazioni stagionali del mix energetico rinnovabile |
| `confronto_prod-fabb.ipynb` | Confronto tra produzione rinnovabile e fabbisogno energetico nazionale |

---

## 📊 Cosa viene analizzato

- Produzione mensile per fonte: **Biomassa, Geotermico, Idrico, Fotovoltaico, Eolico**
- **Copertura percentuale** del fabbisogno nazionale coperta dalle rinnovabili
- **Stagionalità** del mix energetico mese per mese
- Evoluzione temporale dal **2021 al 2026**

### Esempi di grafici prodotti

- Grafico area: produzione rinnovabile vs fabbisogno energetico nel tempo
- Bar chart stacked: mix energetico mensile (analisi stagionale)
- Pie chart: distribuzione media annuale per fonte
- Grafici individuali per ciascuna fonte rinnovabile (esportati in PDF)

---

## 🗂️ Dati utilizzati

- **Fonte:** [Terna – Transparency Report](https://www.terna.it/it/sistema-elettrico/transparency-report)
- **Periodo:** Gennaio 2021 – Febbraio 2026
- **Granularità originale:** Oraria → aggregata a livello mensile
- **File principali:**
  - `Generazione_20XX.xlsx` — dati grezzi anno per anno
  - `Rinnovabili_Pulito:Mesi_2021_2026.csv` — dataset pulito mensile
  - `Fabbisogno_Energetico_Mensile.csv` — fabbisogno nazionale mensile

---

## 🛠️ Tecnologie

- **Python 3**
- `pandas` — manipolazione e pulizia dati
- `matplotlib` — visualizzazioni
- `openpyxl` — lettura file Excel
- **Jupyter Notebook**

---

## 🚀 Come eseguire il progetto

```bash
# 1. Clona il repository
git clone https://github.com/agostomatteo/analisi-rinnovabili.git
cd analisi-rinnovabili

# 2. Installa le dipendenze
pip install pandas matplotlib openpyxl jupyter

# 3. Avvia Jupyter
jupyter notebook
```

Apri i notebook **nell'ordine consigliato**:
1. `Analisi_Rinnovabili.ipynb` (genera i CSV puliti)
2. Gli altri notebook in qualsiasi ordine

---

## 📝 Note

Progetto realizzato per scopi personali e di apprendimento.
I dati sono pubblici e liberamente accessibili dal sito di Terna.
