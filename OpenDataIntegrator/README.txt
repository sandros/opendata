Nuova versione con aggiornamento API e inserimento di nuove funzionalità per gestire l'inserimento e l'aggiornamento dei file tipo ESRI.
Il command code da usare è INSFILEGIS per l'inserimento e UPDFILEGIS per l'aggiornamento.
Il file da usare è uno shape file standard (zip)
Attenzione,
personalizzare i path presenti dentro i due file contenuti nella cartella configs e nel file run.bat.
Aggiungere le cartelle che dovranno contenere i file da pubblicare, i logs e i file eventualmente archiviati.
Le cartelle da creare sono :
- dati
- logs
- archivio
- tracciato_dataset (nuova funzionalità del tool di pubblicazione per un xml dei file processati)

Per sistemi linux dovrà essere anche opportunamente modificato il file per l'esecuzione batch.
