# Repositorio campusciff Ejercicios git

**2.1**.- Crear repository campusciff en git hub
![Alt "Crear Repository Github"](/images/crearRepositorio.jpg)

**2.2**.- Clonar repositorio campusciff en local

    git clone git@github.com:Miriam-Asenjo/campusciff.git


**2.3**.-Crear (si no lo habéis creado ya) en vuestro
repositorio local un documento README.md.

El fichero readme.md se creo al crear el repositorio en github seleccionando checkbox "Initialize this repository with a README" 

**2.4**.- Commit Inicial.

    git add .
    git commit -m "commit inicial"

**2.5**.- Push inicial

    git push origin master

**2.6**.- Ignorar archivos (I)

	touch privado.txt
	mkdir privada 

**2.7**.- Ignorar archivos (II)

    vi .gitignore
   Add entries .gitignore file
![Alt "Modificar .gitignore file"](/images/entriesGitIgnoreFile.jpg)

	git add .
	git commit -m "añadiendo fichero .gitignore"

**2.8**.- Añadir fichero 1.txt

    touch 1.txt
    git add .
    git commit -m "añadir fichero 1.txt"

**2.9**.- Crear el tag v0.1

	git tag v0.1

**2.10**.- Subir el tag v0.1

    git push --tag origin master

**2.11**.- Crear una rama v0.2

    git branch v0.2
    git checkout v0.2

**2.12**.- Añadir fichero 2.txt rama v0.2
	
	touch 2.txt
	git add .
    git commit -m "añadido fichero 2.txt"

**2.13**.- Subir los cambios al repositorio remoto

    git push origin v0.2

**2.14**.- Merge directo

    git checkout master
    git merge v0.2 -m "merge rama v0.2 en master"

**2.15**.- Merge con conflicto (I)
	
	echo "Hola" >> 1.txt
    git add .
    git commit -m "Añadir Hola fichero 1.txt"

**2.16**.- Merge con conflicto (II)
	
	git checkout v0.2
    echo "Adios" >> 1.txt
	git add .
	git commit -m "Añadir Adios fichero 1.txt"

**2.17**.- Merge con conflicto (III)

    git checkout master
	git merge v0.2 -m "merge branch v0.2 en master"

![Alt "Conflicto merge"](/images/mergeConflicto.jpg)


**2.18**- Listado de Ramas
	
	git branch --merged
	git branch --no-merged

**2.19**.- Arreglar conflicto anterior

   Resolver conflictos merge manualmente

	vi 1.txt

![Alt "Resolver conflictos merge manualmente"](/images/resolverConflictosMergeManualmente.jpg)

    git add .
    git commit -m "conflictos merge resueltos"

**2.20**.- Borrar rama

    git tag v0.2
    git branch -d v0.2

**2.21**.- Listado de cambios
	
	git log --oneline --decorate --graph --all

![Alt "Resolver conflictos merge manualmente"](/images/listadoCambios.jpg)

**2.22**.- Cuenta de GitHub

![Alt "Profile Picture GitHub"](/images/gitHubProfilePic.jpg)

![Alt "Enable two factor authentication"](/images/twoFactorAuthentication.jpg)

![Alt "SSH Key Computer"](/images/sshKey.jpg)

**2.23**.- Uso social de GitHub
Siguiendo los siguientes perfiles de compañeros del máster
[GitHub Perfil Danielobit](https://github.com/Danielobit) , 
[GitHub Perfil ADiazGalache](https://github.com/adiazgalache) , 
[GitHub Perfil Macarena Gararena](https://github.com/macarenagaranena)

Siguiendo los repositorios campus ciff de los siguientes compañeros y start them
[Repositorio campusciff Danielobit](https://github.com/Danielobit/campusciff) , 
[Repositorio campusciff ADiazGalache](https://github.com/adiazgalache/campusciff) , 
[Repositorio campusciff Macarena Gararena](https://github.com/macarenagaranena/campusciff)

**2.24**.- Crear una tabla

| NOMBRE              | GITHUB        |
|:--------------------|:------------- |
| Alejandro Diaz      | [Enlace Perfil GitHub](https://github.com/adiazgalache)|
| Daniel Escuder Vieco| [Enlace Perfil GitHub](https://github.com/Danielobit)|
| Macarena Garañena   | [Enlace Perfil GitHub](https://github.com/macarenagaranena)|

**2.25**.- Colaboradores

![Alt "Añadir colaborador repositorio campusciff"](/images/addColaboradorRepositorio.jpg)

**2.26**.- Crear una organización

![Alt "Crear Organizacion"](/images/campusCiff-MiriamAsenjoOrganizacion.jpg)

**2.27**.- Crear equipos
![Alt "Crear Equipos"](/images/equiposGitOrganizacion.jpg)

**2.28**.- Crear un index.html 
Crear repositorio campusciff-miriam-asenjo.github.io en organización campus ciff
incluyendo fichero index.html

[Enlace Página web Organización CampusCiff-Miriam-Asenjo](http://campusciff-miriam-asenjo.github.io./)

**2.29**.- Crear Pull Requests
Realizo fork sobre dos repositorios de compañeros
[Enlace Repositorio 1 ](https://github.com/campusciff-Danielobit/campusciff-Danielobit.github.io)
[Enlace Repositorio 2 ](https://github.com/campusciff-macarenagaranena/campusciff-macarenagaranena.github.io)

Clono el segundo for y añado un cambio
  
    git clone git@github.com:Miriam-Asenjo/campusciff-macarenagaranena.github.io.git
    git branch miriamchanges
	git checkout miriamchanges
	
añado mi nombre en fichero index.html

    git add .
    git commit -m "miriam: aniado mi nombre en index.html"
    git push origin miriamchanges

Pull Request
![Alt "Pull Request"](/images/pullRequest1.jpg)

**2.30** Aceptar los Pull Request que lleguen a mi organizacion

Ejemplo PullRequest sobre repositorio campusciff-Miriam-Asenjo.github.io por el usuario ciffSara 

    git checkout -b campusciff-ciffSara-ramaSara master
    git pull https://github.com/campusciff-ciffSara/campusciff-Miriam-Asenjo.github.io.git ramaSara

	git checkout master
	git merge --no-ff campusciff-ciffSara-ramaSara
	git push origin master

Ejemplo PullRequest sobre repositorio campusciff-Miriam-Asenjo.github.io por el usuario ciffcesarhernandez

    git checkout -b campusciff-ciffcesarhernandez-brCESAR master
    git pull https://github.com/campusciff-ciffcesarhernandez/campusciff-Miriam-Asenjo.github.io.git brCESAR
Conflictos auto-merge failed

	vi index.html
	git add .
	git commit -m "resolving conflict in index.html"

    git checkout master
	git merge --no-ff campusciff-ciffcesarhernandez-brCESAR
    git push origin master
