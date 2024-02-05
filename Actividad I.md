# ACTIVIDAD I: Ejercicio de creación y actualización de repositorios


## EJERCICIO I
		
1. Crear un repositorio nuevo con el nombre “Libro” y mostrar su contenido
	***mkdir Libro***

	***cd Libro/***

	***git init***
	
	***ls -la***

2. Configurar Git definiendo el nombre de usuario, el correo electrónico y activar la salida en color. Mostrar la configuración final.

	***git config --global user.name “Andrea B Mendez”***
	
	***git config --global user.email “andbermen@alu.edu.gva.es”***
	
	***git config --global color.ui auto***

			    
			    
	***git config --list***

	***git config --global --list***
	
	***git config --local --list***





## EJERCICIO II
1. Comprobar el estado del repositorio
	
	***git status***

2. Crear un fichero index.txt con el siguiente contenido:

	***cat > indext.txt***
	
	    Capítulo 1: Introducción a Git
	    
	    Capítulo 2: Flujo de trabajo básico
	    
	    Capítulo 3: Repositorios remotos
	    
	***ctrl+D***

3. Comprobar nuevamente del estado del repositorio

	***git status***

4. Añadir fichero a la zona de intercambio temporal.
	
	***git add index.txt***

5. Comprobar una vez más el estado del repositorio

	***git status***


   
	
## EJERCICIO III
1. Realizar un commit de los últimos cambios con el mensaje «Añadido índice del libro» y comprobar el estado del repositorio.

	***git commit -m "Añadido índice del libro"***
	
	***git status***




## EJERCICIO IV
1. Cambiar el fichero index.txt con la siguiente información

	***cat > index.txt***
			
		Capítulo 1: Introducción a Git
				
		Capítulo 2: Flujo de trabajo básico
			
		Capítulo 3: Gestión de ramas
				
		Capítulo 4: Repositorios remotos
		
	***ctrl+D***

2. Mostrar los cambios respecto a la última versión guardada en el repositorio

	***git diff***

3. Hacer  un commit de los cambios con el mensaje «Añadido capítulo 3 sobre gestión de ramas.»

	***git commit -m "Añadido capítulo 3 sobre gestión de ramas."***


## EJERCICIO V
1. Mostrar los cambios de la última versión del repositorio con respecto a la anterior

	***git show***

2. Cambiar el mensaje del último commit a «Añadido capítulo sobre gestión de ramas al índice.»

	***git commit --amend -m "Añadido capítulo sobre gestión de ramas al índice."***

3. Volver a mostrar los últimos cambios del repositorio

	***git show***


   

## EJERCICIO VI
Indica a git que quieres ignorar todos los ficheros que empiezar por «daw», todos los que tienen la extensión out y las imágenes (jpg, png, bmp y gif)

	nano .gitignore
	
	#Ignorar archivos que comienzan con "daw"
	
	daw*
	
	#Ignorar archivos con extensión ".out"
	
	*.out
	
	#Ignorar imágenes con extensiones ".jpg", ".png", ".bmp" y ".gif"
	
	*.jpg
	
	*.png
	
	*.bmp
	
	*.gif
 
	
   ***git add .gitignore***
	
   ***git commit -m "Archivo gitignore añadido."***

