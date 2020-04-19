---------------------------------------------------------------------
---------- ---------- ESTADO, STAGGIN-INDEX, COMMIT  ----------
---------------------------------------------------------------------
git status

git add index.html
git add .
	Poner todos los ficheros modificados en el staggin-index

git rm --cached [nombre_fichero]
	Eliminamos [nombre_fichero] del staggin-index

.gitignore
	Archivo para indicar los tipos de archivo y archivos concretos que serán ignorados por Git

git commit -m "Descripción de la versión"

---------------------------------------------------------------------
---------- ---------- HISTORIAL DE CAMBIOS ---------- ----------
---------------------------------------------------------------------
git log

git log --stat
	Muestra el historial de commits

git log --oneline
	Muestra el histórico de commits, cada uno en una línea

git log --graph
	Muestra el histórico de commits y las ramas de forma gráfica

git log --oneline --graph --all	
	Muestra el histórico de commits en una línea y las ramas de forma gráfica

git diff
	Muestra diferencias desde el último commit

git diff <número de commit> [nombre_fichero]
	Muestra las diferencias del archivo actual con el archivo de la versión del commit

git checkout <número de commit>
	Regresamos a la versión del commit (se pierden todos los cambios realizados posteriormente)

---------------------------------------------------------------------
---------- ---------- RAMAS ---------- ----------
---------------------------------------------------------------------
git branch
	Muestra todas las ramas

git checkout [nombre_rama]
	Cambiar a la rama [nombre_rama]

git checkout -b [nombre_rama]
	Crear nueva rama [nombre_rama]

git merge [nombre rama]
	Combina la rama en la que nos encontramos con [nombre_rama]

git branch -d [nombre_rama]
	Borrar rama [nombre_rama]

---------------------------------------------------------------------
---------- ---------- GITHUB ---------- ----------
---------------------------------------------------------------------

…Create a new repository on the command line
echo "# curso_desarrollo_web" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/lagunaprofesional/curso_desarrollo_web.git
git push -u origin master
--

…or push an existing repository from the command line
git remote add origin https://github.com/lagunaprofesional/curso_desarrollo_web.git
	Enlazar nuestro repositorio local con Github

git push -u origin master
	Subir cambios desde nuestro repositorio local a Github
--

git pull origin master
	Bajar cambios desde Github hacia nuestro repositorio local (laptop)
