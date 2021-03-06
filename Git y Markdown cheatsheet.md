**Eliminar un directorio de git**  
```
rm -rf <directorio>
```

**Mostrar código para diferentes lenguajes**  
C:
```c
int main () {
    printf("Hola!");
}
```
## Creando una nueva *branch* y haciendo una *pull request*
Una vez que tenemos el repositorio clonado localmente, creamos una nueva *branch* y nos pasamos a ella:  
```bash
git checkout -b <nombreRama>
```  
Luego de realizar los cambios, los agregamos y realizamos el commit:  
```bash
git commit -a -m "Mensaje"
```  
Realizamos el *push*. La primera vez hay que setear el upstream:  
```bash
git push --set-upstream origin <nombreRama>
```  
Luego ya se puede hacer un *pull request* para que los cambios que realizamos en la rama nueva, pasen a la rama *main*. Esto se hace directamente desde GitHub.  
Los colaboradores del repositorio pueden administrar los *pull request*.  
Una vez que ya se realizó el *merge* de la *branch*, ya se pueden eliminar.  

## Eliminando ramas que creamos
Eliminar rama localmente
```bash
git branch -d <nombreRama>
```

Eliminar rama remotamente
```bash
git push origin --delete remoteBranchName
```  
Una vez eliminadas las ramas, hay que eliminar el *tracking* a las mismas:  
```bash
git remote prune origin
```
```bash
git prune
```

Martes
is

Miércoles
lab
is

Jueves
lab

Viernes
presentar todo
ale

Sábado
walidapp
