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
Una vez que tenemos el repositorio clonado localmente, se pasa a crear una nueva *branch* y pasarnos a ella:  
```bash
git checkout -b <nombreRama>
```  
Luego de realizar los cambios, agregarlos y realizar el commit:  
```bash
git commit -a -m "Mensaje"
```  
Realizar el *push*. La primera vez hay que setear el upstream:  
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
