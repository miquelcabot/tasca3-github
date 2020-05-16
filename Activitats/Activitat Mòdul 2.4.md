#  Activitat Mòdul 2.4

En aquesta activitat, se us demanarà que resolgueu un conflicte de *merge*. Volem crear un `README.md` que digui `"Hello World"`.

Copieu i enganxeu aquestes ordres a la vostra línia de comandes i pitgeu `return`:

```
mkdir MergeConflict
cd MergeConflict/
git init
touch README.md
echo "echo Hello" > README.md
git add .
git commit -m"first commit on master"
git checkout -b new-branch
echo "Hello World" > README.md
git add .
git commit -m"first commit on new-branch"
git checkout master
echo "Hola" > README.md
git add .
git commit -m"second commit on master"
git merge new-branch
```

Aquest "script" crearà un conflicte de *merge*. Resoleu el conflicte de *merge* perquè el text a `README.md` sigui `"Hello World"`.

Feu una captura de pantalla de la vostra línia d'ordres que mostri que heu resolt el conflicte de *merge* i pengeu la captura de pantalla a un nou `Issue` titulat `Activitat Mòdul 2.4`.
