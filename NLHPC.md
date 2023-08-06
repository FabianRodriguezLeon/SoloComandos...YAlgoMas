# Comados del servidor

| Comando | Función                                               |
|-----------------------|-------------------------------------------------------|
| sinfo                   | Muestra el estado de las particiones.                         |
| squeue                    | Muestra la cola de tareas. Se puede especificar con -usuario.                           |
| sbatch "script.sh"                | Manda a correr un script en el backend.                                 |
| srun         | Corre un script en el frontend.                                      |
| scancel                   | Ver manual de un comando.                              |
| sacct -X                 | Muestra el estado de todas las tareas ejecutadas.                               |
| scontrol -dd show “ID del trabajo”                | Detalla la información de un trabajo/script.                                |
| sstat                   | Muestra la cantidad de recursos utilizados por un trabajo/script.                       |
| scontrol write batch_script <job_id>                    | Ver el script asociado a un trabajo.       |
 
# Variables de SLURM

| Parámetro | Significado                                               |
|-----------------------|-------------------------------------------------------|
| -p “partición”                  | Enviar un trabajo a una partición en específico. Por default se envia a la partición slims.                        |
| -n “número de núcleos“                   | Número de tareas que serán asignadas para correr un trabajo/script.                            |
| -c “Número de nodos”                   | Esta es la cantidad de CPU que necesita el trabajo/ script. El valor predeterminado es 1 CPU.                                 |
| --mem-per-cpu=“Valor”                 | Memoria en Mb que usará el CPU para correr el script/trabajo. Por default es 1 Gb o 1024 Mb.                                      |
| -o “NombredelArchivo_%j.out”                   | Es el output que resulta de correr el script. %j detalla el Job ID del script/trabajo.                              |
| -e “NombredelArchivo_%j.err”                  | Crea un archivo que especifica si hubo algún error al correr el script.                               |
| -t “Dias-Horas:Minutos:Segundos”                | Tiempo de corrida aproximado para el script.                                 |
| -J “Nombredeltrabajo”                    | Le da nombre al trabajo.                      |




# Especificaciones Guacolda-Leftraru

| Partición | Detalle                                               |
|-----------------------|-------------------------------------------------------|
| Leftraru nodo slim (cn)                   | 132 nodos (264sinfo: Muestra el estado de las particiones.                         |
| Guacolda nodo general (sn)                    | 48 nodos (2112 núcleos).                             |
| Guacolda nodo Largemen (fn)                    | 9 nodos (396 núcleos).                                 |
| Guacolda nodo GPU (gn)                | 2 nodos.                                      |


# Especificaciones de las particiones

Cuando lanzamos el comando squeue podemos ver el estado de las particiones slim, general, Largemen, GPU entre otras. Dependiendo de la cantidad de núcleos usados en cada partición se despliega alguno de los siguientes mensajes. 

| Mensaje | Significado                                               |
|-----------------------|-------------------------------------------------------|
| Idle                   | Todos los núcleos están desocupados.                         |
| Mix                  | Existen núcleos disponibles y otros ocupados.                             |
| Alloc                    | Todos los núcleos se encuentran ocupados.                                |

