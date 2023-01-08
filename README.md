# ScreenCaptureOCR
ScreenCaptureOCR (Optical Character Recognition) è un progetto scritto in python che cattura una parte dello schermo e estrae il testo il quale sarà disponibile per essere incollato (Ctrl+v).
Funziona solo per i sistemi operativi Windows.

## Requisiti

Per eseguire questo progetto, sarà necessario avere installato:

- [Python](https://www.python.org/downloads/) (è stato testato con la versione 3.9)
- [pytesseract](https://pypi.org/project/pytesseract/) (è stato testato con la versione 0.3.10)
- [pip](https://pip.pypa.io/en/stable/installing/) (viene installato insieme a Python)

**Nota:** Questo progetto è stato testato solo su Windows10Pro.

## Installazione

1. Python: è possibile scaricare l'ultima versione di Python da https://www.python.org/downloads/
2. Tesseract, un software open source per l'OCR. Per installare tesseract su Windows, seguire questi passaggi:
- Vai al sito web di tesseract: https://github.com/UB-Mannheim/tesseract/wiki e scarica la tua versione.
- Una volta scaricato il file .exe, eseguilo per installare tesseract sul tuo computer.
- Assicurati di aggiungere il percorso di Tesseract al tuo PATH di sistema. Per fare ciò, vai su "Pannello di controllo" -> "Sistema" -> "Impostazioni di sistema avanzate" -> "Variabili d'ambiente". Nella sezione "Variabili di sistema", seleziona la variabile "Path" e clicca su "Modifica". Aggiungi il percorso di Tesseract al PATH (ad esempio, "C:\Program Files (x86)\Tesseract-OCR")
3. Scaricare il progetto git `git clone https://github.com/bestrus/ScreenCaptureOCR.git`
4. Aprire il prompt dei comandi nella cartella del progetto e digitare il seguente comando per installare le dipendenze del progetto:
`pip install -r requirements.txt`

## Esecuzione

```
$ git clone https://github.com/bestrus/ScreenCaptureOCR.git
$ cd ScreenCaptureOCR
$ python -m venv .venv
$ .venv\Scripts\activate.bat
$ pip install -r requirements.txt
$ python screen_capture.py
```