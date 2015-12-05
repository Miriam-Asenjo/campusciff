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