# ACTIVIDAD III: Deshacer cambios

## EJERCICIO I
1. Elimina la última línea del fichero índice.txt y guárdalo
   
    ***nano index.txt***

3. Comprueba el estado del repositorio
   
	***git status***

5. Deshaz los cambios realizados al fichero índice.txt para volver a la versión anterior del fichero
   
	***git checkout-- index.txt***

7. Vuelve a comprobar el estado del repositorio
   
	***git status***

## EJERCICIO II
1. Elimina la última línea del fichero índice.txt y guárdalo
   
	***nano index.txt***

2. Añade los cambios en la zona de intercambio temporal
   
    ***git add .***

3. Comprueba de nuevo el estado del repositorio
   
    ***git status***

4. Saca los cambios de la zona de intercambio temporal, pero  manteniendolos al directorio de trabajo
   
    ***git reset index.txt***

5. Comprueba de nuevo el estado del repositorio
    
    ***git status***

6. Deshaz los cambios realizados al fichero índice.txt para volver a la versión anterior del fichero
    
    ***git checkout -- index.txt***

7. Vuelve a comprobar el estado del repositorio
    
    ***git status***
		
## EJERCICIO III
1. Elimina la última línea del fichero índice.txt y guardarlo

    ***nano index.txt***
   
3. Elimina el fichero Capítulos/capitulo3.txt
		
    ***git rm Capítulos/capitulo3.txt***
  
4. Añade un fichero nuevo Capítulos/capitulo4.txt vacío
		
    ***cat > Capítulos/capitulo4.txt***
		
    ***ctrl+D***
5. Añade los cambios en la zona de intercambio temporal
		
    ***git add .***
  
6. Comprueba de nuevo el estado del repositorio

    ***git status***

8. Saca los cambios de la zona de intercambio temporal, pero mantenlos en  el directorio de trabajo

    ***git reset***

10. Comprueba de nuevo el estado del repositorio
		
    ***git status***
  
11. Deshaz los cambios realizados para volver a la versión del repositorio
		
    ***git checkout -- .***
  
12. Vuelve a comprobar el estado del repositorio
		
    ***git status***

## EJERCICIO IV
1. Elimina la última línea del fichero index.txt y guardarlo

    ***nano index.txt***

3. Elimina el fichero Capítulos/capitulo3.txt

    ***git rm Capítulos/capitulo3.txt***

5. Añade los cambios en la zona de intercambio temporal y hacer un commit con el mensaje "Borrado accidental."

    ***git commit -m “Borrado accidental”***

7. Comprueba el historial del repositorio

    ***git log***

9. Deshaz el último commit, pero manten los cambios anteriores al directorio de trabajo y en la zona de intercambio temporal

    ***git reset --soft HEAD~1***

11. Comprueba el historial y el estado del repositorio
		
    ***git status***
  
12. Vuelve a hacer el commit con el mismo mensaje de antes
		
    ***git commit -m “Borrado accidental”***
  
13. Deshaz el último commit y los cambios anteriores al directorio de trabajo, volviendo a la versión anterior del repositorio
		
    ***git reset --hard HEAD~1***
  
14. Comprueba de nuevo el historial y el estado del repositorio
		
    ***git log***
  
    ***git status***
