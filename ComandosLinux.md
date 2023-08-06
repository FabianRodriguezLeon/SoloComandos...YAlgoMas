# COMANDOS INTERESANTES DE LINUX Y SUS ARGUMENTOS

1) **grep** “Expresión” “Archivo”: Global regular expresion print

	-i: Anula la sensibilidad de busqueda (i.e, mayusculas, comas, etc).

	-r: Busca recursivamente en todos los subdirectorios del directorio actual.

	-c: Cuenta el número total de líneas en donde aparece la expresión de interés.

	--color: Destaca la expresión buscada en un color en específico.
   
	--help: Listado en detalle de los argumentos de grep.

3) **wc**: Word count

	-l: Muestra el número de líneas del archivo.

	-w Imprime el número total de palabras del archivo.

	-m: Imprime el número total de caracteres del archivo.

5) **sed**: Stream editor. Entre sus funciones más importantes se encuentran: buscar, buscar y reemplazar, insertar o eliminar.

	Ejemplo Poema de Federico García Lorca Romance Noctámbulo del repositorio: 

	sed 's/Compadre/Amigo mío/' verde.txt 

	Este comando va a buscar la expresión “Compadre” en el archivo verde.txt y la va a reemplazar por “Amigo mío”.

6) **gsub()**: Global substitution. Es una función de Strings que permite buscar y reemplazar texto.

	Ejemplo: gsub("letra_palabra_o_expresión_regular_a_buscar", "texto_que_reemplaza_el_buscado", lugar_donde_realizar_sustitución)

7) **awk**: Comando bien bien importante. En términos generales awk permite procesar y modificar el texto según diversas necesidades.

	Algunos ejemplos

	i) Procesar texto y mostrar las líneas y columnas que cumplen con determinadas condiciones.

	awk '{print $num_columna}' Archivo

	-F “'Delimitador'”: Fija una delimitador 

	ii) Buscar palabras y patrones de palabras y reemplazarlos por otras palabras y/o patrones.

	iii) Hacer operaciones matemáticas.

8) **find**: Encuentra archivos en el sistema

	Ejemplo: find "Ruta absoluta" -name '*reportes*.doc'

	-name: Le indica a find que use el patrón provisto para buscar en los nombres de archivo.

	Existe un comando similar llamado locate.

9) **whereis**: Busca dentro del sistema comandos y manuales basándose en los parámetros de búsqueda provistos 

	Ejemplo: whereis bash 
	        » bash: /usr/bin/bash 

10) **du**: Disk usage

	-s: Muestra el peso total de un archivo/ directorio.

	-h: Muestra el peso del archivo en un formato coherente (Mb, Gb, etc ).

12) **ls**: List

	-R: Lista todos los archivos en el subdirectorio.

	-a: Muestra archivos que estén ocultos.

	-lh: Lista los archivos y muestra su peso.

14) cd: Change directory

	cd .. : Te mueve un directorio hacia atras.

	cd: Te devuelve al home.

16) **cp** "Archivo" “Ruta”: Copy

	-R: Copia todo el directorio actual

17) **mv**: Move. Permite mover de directorio y cambiar de nombre a archivos/directorios.

18) **rmdir**: Remove directory (que estén vacios)

19) **rm**: Remove (Para siempre!!)

	-r: Borra directorios y archivos de forma recursiva (estén o no vacios).

	-i: Pregunta antes de cada borrado.
 
	-f: Mata los ficheros y argumentos que no existan, sin preguntar.

21) **curl**: Client url

	-O: Usa la vesion HTTP 1.0.

	-J: Conserva el encabezado (header) especificado po el servidor en vez de el obtenido desde la URL.

	-X: Especifica el método de comunicación requerido con el servidor.

23) **wget**: World Wide Web get 

24) **history**: Muestra el historial de comandos

	-c: Borra el historial de comandos

25) **clear**: Limpia la salidas/pantalla de la terminal.

26) **zip**: Comprime un archivo

27) **unzip**: Descomprime un archivo

28) **mkdir**: Make directory

29) **pwd**: Print working directory

30) **nano**: Editor de texto plano. 

31) **chmod +x**: Change mode. Convierte un archivo en un script ejecutable. Recordar siempre incluir la extensión .sh del script.

32) **man**: Manual. Despliega el manual del comando de interés. 












