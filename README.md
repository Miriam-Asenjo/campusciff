# Repositorio campusciff Ejercicios git

2.1.- Crear repository campusciff en git hub
![Alt "Crear Repository Github"](/images/crearRepositorio.jpg)

2.2.- Clonar repositorio campusciff en local

    git clone git@github.com:Miriam-Asenjo/campusciff.git


2.3.-Crear (si no lo habéis creado ya) en vuestro
repositorio local un documento README.md.

El fichero readme.md se creo al crear el repositorio en github seleccionando checkbox "Initialize this repository with a README" 

2.4 Commit Inicial.

    git add .
    git commit -m "commit inicial"

2.5 Push inicial

    git push origin master

2.6 Ignorar archivos (I)

	touch privado.txt
	mkdir privada 

2.7 Ignorar archivos (II)

    vi .gitignore
   Add entries .gitignore file
![Alt "Modificar .gitignore file"](/images/entriesGitIgnoreFile.jpg)

	git add .
	git commit -m "añadiendo fichero .gitignore"

2.8 Añadir fichero 1.txt

    touch 1.txt
    git add .
    git commit -m "añadir fichero 1.txt"

2.9 Crear el tag v0.1

	git tag v0.1

2.10 Subir el tag v0.1

    git push --tag origin master

2.11 Crear una rama v0.2

    git branch v0.2
    git checkout v0.2

2.12 Añadir fichero 2.txt rama v0.2
	
	touch 2.txt
	git add .
    git commit -m "añadido fichero 2.txt"

2.13 Subir los cambios al repositorio remoto

    git push origin v0.2