# ACTIVIDAD IV: Gestión de ramas
### EJERCICIO I
1. Crea una nueva rama bibliografía y mostrar las ramas del repositorio.
   
    ***git branch bibliografia***

### EJERCICIO II
1. Crear el fichero Capítulos/capitulo4.txt y añadir el siguiente texto:
   
    ***cat > Capítulos/capitulo4.txt***
   
          En este capítulo veremos como utilizar GITHUB para alojar repositorios remotos.
   
    ***Ctrl + d***
   
2. Añadir los cambios en la zona de intercambio temporal.
   
    ***git add .***
   
3. Hacer un commit con el mensaje "Añadido capítulo 4."
 
    ***git commit -m "Añadido capítulo 4."***
   
4. Mostrar la historia del repositorio incluyendo todas las ramas.
   
    ***git log***

### EJERCICIO III
1. Cambia a la rama bibliografía.

   ***git checkout bibliografia***
   
3. Crea el fichero bibliografía.txt y añadir la siguiente referencia:
    ***cat > bibliografia.txt***
   
       - Chacon, S. and Straub, B. Pro Git. Apress

   ***Ctrl+d***

3. Añade los cambios en la zona de intercambio temporal.

    ***git add .***
   
5. Fez un *commit con el mensaje "Añadida primera referencia bibliográfica."

    ***git commit -m "Añadida la primera referencia bibiográfica."***
   
7. Muestra la historia del repositorio incluyente todas las ramas.

    ***git log --graph --all –oneline***

### EJERCICIO IV
1. Fusiona la rama bibliografía con la rama master.

    ***git checkout master***
   
    ***git merge bibliografia***
   
3. Muestra la historia del repositorio incluyente todas las ramas.

    ***git log --graph --all --oneline***
   
5. Elimina la rama bibliografía.

    ***git branch -d bibliografia***
   
7. Muestra de nuevo la historia del repositorio incluyente todas las ramas.

    ***git log --graph --all –oneline***

### EJERCICIO V
1. Crea la rama bibliografía.

    ***git branch bibliografia***
   
3. Cambia a la rama bibliografía.

    ***git checkout bibliografia***

4. Cambia el fichero bibliografía.txt para que contenga las siguientes referencias:

    ***git nano***
                   
         - Scott Chacon Ben Straub. Pro Git. Apress
         - Ryan Hodson. Ry's Git Tutorial. Smashwords (2014)
  
4. Añade los cambios en la zona de intercambio temporal y hacer un commit con el mensaje "Añadida nueva referencia bibliográfica."

    ***git add .***
    
    ***git commit -m "Añadida nueva referencia bibliográfica."***

5. Cambia a la rama master.

    ***git checkout master***
   
7. Cambia el fichero bibliografía.txt para que contenga las siguientes referencias:

   ***nano bibliografia.txt***
     
         - Chacon, S. and Straub, B. Pro Git. Apress
         - Loeliger, J. and McCullough, M. Version control with Git. O'Reilly
  
7. Añade los cambios en la zona de intercambio temporal y hacer un commit con el mensaje "Añadida nueva referencia bibliográfica."

    ***git add .***

    ***git commit -m “Añadida nueva referencia bibliografica.”***

8. Fusiona la rama bibliografía con la rama master.

    ***git merge bibliografia***
  
9. Resuelve el conflicto dejando el fichero bibliografía.txt con las referencias:

    ***nano bibliografia.txt***
   
          - Chacon, S. and Straub, B. Pro Git. Apress
          - Loeliger, J. and McCullough, M. Version control with Git. O'Reilly
          - Hodson, R. Ry's Git Tutorial. Smashwords (2014)

11. Añade los cambios en la zona de intercambio temporal y haz un commit con el mensaje "Resuelto conflicto de bibliografía."

      ***git add .***
      ***git commit -m "Resuelto conflicto de bibliografía."***
    
13. Muestra la historia del repositorio incluyendo todas las ramas.

      ***git log --graph --all --oneline***
