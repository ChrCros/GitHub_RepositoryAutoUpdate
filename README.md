"# GitHub_RepositoryAutoUpdate" 
# GUIDA RAPIDA SU COME CARICARE ED AGGIORNARE IN MANIERA AUROMATICA UNA REPOSITORY SU https://github.com/

## Creare una nuova repository dalla riga di comando
```sh
echo "# GitHub_RepositoryAutoUpdate" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/ChrCros/GitHub_RepositoryAutoUpdate.git
git push -u origin main
```

## Eseguire l'aggiornamento di una repository esistente dalla riga di comando
```sh
git remote add origin https://github.com/ChrCros/GitHub_RepositoryAutoUpdate.git
git branch -M main
git push -u origin main
```
