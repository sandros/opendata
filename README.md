# Esempio di utilizzo di Kettle per pubblicare un nuovo dataset in opendata, oppure aggiornarne il contenuto.
Nel file .kettle.properties deve essere valorizzata la variabile ETL_PATH (attenzione, è case sensitive), con il percorso in cui si salvano i file di questo esempio ed il tool di pubblicazione.
Possiamo pensare di valorizzarla ad esempio a "C:\OpenDataIntegrator\" se su Windows, oppure "../OpenDataIntegrator/" se su linux
I file contengono una serie di oggetti che eseguono le seguenti attività:
- cancellazione dei vecchi file di processo presenti nella cartella
- esecuzione del backup del dataset attualmente pubblicato
- unione di due file di tipo foglio di lavoro in un unico file csv con l'aggiunta di una informazione specifica relativa al file sorgente
- creazione dinamica del file xml necessario al tool di pubblicazione (con possibilità di definizione dei metadati e della larghezza delle colonne pubblicate)on the fly
- spostamento dei file necessari al tool di pubblicazione nella sua cartella di lavoro
- invio tramite mail del risultato della pubblicazione, basato sul log creato dal tool.
Per utilizzare gli esempi pubblicati, è necessario :
- avere configurato una JAVA openjdk (versione 7 o 8 al momento della scrittura di queste note)
- avere scaricato Kettle (o Pentaho) ETL disponibile a questo link : http://community.pentaho.com/projects/data-integration/
- S.O. Windows o Linux/Unix (non è stato testato su piattaforma MacOS X)

DISCLAIMER
Gli elementi sono forniti AS IS, con licenza IODL 2.0 e sono a puro titolo di esempio.
I software necessari all'utilizzo di questi esempi, sono assoggettati al Copyright ed alle licenze d'uso definite dal produttore del software.
