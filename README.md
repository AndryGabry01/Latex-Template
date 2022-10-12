# Latex Template
### Funzionamento
1) Inserire i proprio appunti, nel file "Appunti.tex"
2) Inserire i propri dati nelle costanti "main.tex" (es \Insegnamento) 
3) Compilare il file "main.tex" per ottenere il file pdf
  !ATTENZIONE!
  Per ottenere un output pulito, ovvero far si che i file di output finiscano in una cartella seprata "Output",
  bisogna modificare le impostazioni utente di vscode "setting.js", inserendo in maniera corretta il contenuto del file situato in 
    "./Config/VSCODESETTING.json"

  Cosi facendo i file di output (*.aux, *.log, ed il file PDF) finiranno in una cartella apposita "Output", piuttosto che venir
  buttati nella cartella principale

  Se tutto è impostato correttamente, dopo la prima compilazione, il filesystem risultera simile a questo:
  ```
   Root
   |-(Dir)Config
     |-(fileconfig)
   |-(Dir)Foto
     |-(fileconfig)
   |-(Dir)Output
     |-(fileconfig)
   |-(File dove inserire i propri appunti)Appunti.tex
   |-(File dove inserire le costanti e da compilare per ottenere il pdf)main.tex
```
### Informazioni
- Nel file main.tex vanno impostate le costanti come \Insegnamento \Corso ed Etc
- Gli appunti vanno inseriti nel file "Appunti.tex"
- Le foto vanno nella cartella "Foto", ed all'interno del codice è possibile usare \foto{filename.tex} in modo tale da non dover inserire ogni volta il Path della cartella "Foto"
- I file di config ed aggiuntivi vanno nella cartella "Config", ed all'interno del codice è possibile usare \config{filename.tex} in modo tale da non dover inserire ogni volta il Path della cartella "Config"
- Per tenere pulito il codice sarebbe buon uso inserire eventuali comandi aggiuntivi nel file "./Config/config.tex"

## Guide ed Editor Online
https://www.overleaf.com/ 

### Segnalazioni
Segnalazioni d'errore e consigli sono bene accetti, poiche questo template è stato creato di fretta e furia. 
