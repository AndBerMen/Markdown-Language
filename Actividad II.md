# ACTIVIDAD II: Uso del historial de cambios

### EJERCICIO I
1. Muestra el historial de cambios del repositorio.

		***cd Libro/***
		***git log***
2. Crea la carpeta capítulos y dentro de ella crea el fichero *capitol1.txt con el siguiente texto:

		***mkdir > Capítulos***
		***cat > Capítulos/capitulo1.txt***
			    Git es un sistema de control de versiones ideado por Linus Torvalds.
		***crtl+D***

3. Añade los cambios en la zona de intercambio temporal (staging area)

		***git add .***

4. Haz un commit de los cambios con el mensaje "Añadido capítulo 1."

		***git commit -m “Añadido capítulo 1.”***

5. Vuelve a mostrar el historial de cambios del repositorio.

		***git log***

### EJERCICIO II

1. Crea el fichero capitulo2.txt en la carpeta capítulos con el siguiente texto:

		***cat > Capítulos/capitulo2.txt***
  			El flujo de trabajo básico con Git consiste en:
  			1 – Hacer cambios en el repositorio
  			2 – Añadir los cambios a la zona de intercambio temporal.
  			3 – Hacer un commit de los cambios
		***crtl+D***
	
2. Añade los cambios en la zona de intercambio temporal.

		***git add .***

3. Haz un commit de los cambios con el mensaje "Añadido capítulo 2."

		***git commit -m “Añadido capítulo 2.”***

4. Muestra las diferencias entre la última versión y las dos versiones anteriores.

		***git diff HEAD~2..HEAD***

### EJERCICIO III

1. Crea el fichero capitulo3.txt en la carpeta capítulos con el siguiente texto:

		***cat > Capítulos/capitulo3.txt***
			    Git permite la cración de ramas, cosa que permite tener distintas 				versiones del mismo proyecto y trabajar de forma simultánea en ellas.
		***crtl+D***

2. Añade los cambios en la zona de intercambio temporal.

		***git add .***

3. Haz un commit de los cambios con el mensaje "Añadido capítulo 3."

		***git commit -m “Añadido capítulo 3.”****

4. Muestra las diferencias entre la primera y la última versión del repositorio.

		***git diff 0f8c48..HEAD***

### EJERCICIO IV
1. Añade al final del fichero index.txt la siguiente línea: “Capítulo 5: conceptos avanzados”

		***nano index.txt***

2. Añade los cambios en la zona de intercambio temporal.

		***git add .***

3. Haz un commit de los cambios con el mensaje "Añadido capítulo 5 al índice."

		***git commit -m “Añadido capítulo 5 al índice.”***

4. Muestra quién ha hecho cambios sobre el fichero índice.txt.

		***git annotate index.txt / git blame index.txt***
