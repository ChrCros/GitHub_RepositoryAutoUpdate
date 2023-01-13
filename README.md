# GUIDA RAPIDA SU COME CARICARE ED AGGIORNARE IN MANIERA AUROMATICA UN PROGETTO SU https://github.com/

## Creare una nuova repository dalla riga di comando
### Creare un repository
> Collegatevi sul sito di github ,se non lo avete, create un profilo, attendete la conferma email ecc…
Quindi create un **repository** (ossia il contenitore del nostro progetto compreso le revisioni dello stesso) cliccando a destra sul tasto verde **new repository** , nella pagina che segue assegnate un nome, ad esempio prova. Se volete date una descrizione del progetto (è opzionale) quindi cliccate su **public** ed infine su **create repository**.
### Caricare un progetto
> Ora che avete creato il repository create il file Readme,anche se opzionale io ve lo consiglio, cliccando su di esso, poi clonate il progetto cliccando su : "C:\Users\AjhanOsmanoski-NewMI\Downloads\Cattura.JPG"
> Create una directory nel vostro pc dove intendete salvare il progetto,quindi aprite Git for Windows recatevi all’interno della cartella creata e digitate
```sh
echo "# GitHub_RepositoryAutoUpdate" >> README.md
git init #crea un repository in locale.
git add README.md #aggiunge il file README.md
git commit -m "first commit" #carichiamo il progetto nell'HEAD di git, 
git branch -M main #sposta il ramo master locale nel ramo main principale
git remote add origin https://github.com/ChrCros/GitHub_RepositoryAutoUpdate.git # Crea un nuovo repository Git vuoto sul tuo server remoto
git push -u origin main #Carica i file selezionati in remoto, tra le virgolette è solo un messaggio per la commit.
```

## Eseguire l'aggiornamento di una repository esistente dalla riga di comando
```sh
git add * #copiare path del file da caricare/aggiornare
git commit -m "first commit"
git branch -M main
git push -u origin main
```
