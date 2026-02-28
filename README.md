# csv explorer

A browser-based tool for quickly exploring CSV files. Drop in any CSV and instantly get column stats, data distributions, and a searchable preview table — no server, no installs, nothing gets uploaded anywhere.

---

## what it does

- drag & drop (or click to browse) any CSV file
- shows an **overview**: row count, column count, missing values, completeness %
- **column profiles** for every column — type detection, min/max/avg for numbers, unique counts for text, missing value bars
- **auto-generated charts** — histograms for numeric columns, bar charts for categorical ones
- **searchable data table** with row limit selector (20 / 50 / 100 / all)
- everything runs in the browser — your data never leaves your machine

---

## how to run it

Just open `index.html` in any modern browser. That's it.

```bash
git clone https://github.com/amanay-codes/csv-explorer.git
cd csv-explorer
# open index.html in your browser
```

No npm, no Python, no server needed.

---

## tech used

- **PapaParse** — for parsing CSV files (handles edge cases way better than doing it manually)
- **Chart.js** — for the distribution charts
- vanilla HTML/CSS/JS for everything else

Both libraries are loaded from a CDN so there's nothing to install.

---

## what kind of CSV files work

Pretty much any standard CSV. Works well with:
- exported spreadsheets (Excel, Google Sheets)
- dataset files from Kaggle or similar
- database exports
- any flat tabular data with a header row

Large files (100k+ rows) might be a bit slow depending on your machine.

---

## project structure

```
csv-explorer/
└── index.html    # the whole app in one file
```

Kept it as a single file on purpose — easier to share, easier to understand.

---

## stuff I want to add eventually

- [ ] column-level filtering (not just row search)
- [ ] export a summary report as PDF
- [ ] correlation matrix for numeric columns
- [ ] detect and highlight outliers

---

made by [amanay-codes](https://github.com/amanay-codes)
