# **Proyecto I**
Trabajo final Algoritmia y programación 2024-1

![image](https://github.com/PrettySusi/Proyecto_I/assets/169689247/ea5d3f58-7821-42b4-a9ce-f5301bbec82a)

**Propósito y Utilidad del Proyecto**
Este proyecto automatiza la creación de una estructura de directorios y archivos para la organización de información académica, simulando un sistema de gestión de estudiantes y materias

**Descripción del Proyecto**

El proyecto está diseñado para procesar y organizar información académica relacionada con materias y estudiantes, a continuación, se describe cada componente y su función:

1. Importación de Bibliotecas
El proyecto utiliza varias bibliotecas de Python para manipulación de datos, manejo de archivos y operaciones matemáticas:
- pandas: Para la manipulación de datos.
- numpy: Para operaciones numéricas.
- random: Para operaciones aleatorias.
- os y pathlib: Para el manejo del sistema de archivos.
- unidecode: Para normalización de texto.

2.Carga de Datos
Se cargan tres conjuntos de datos:
- Materias, Semestre y Créditos:Información sobre las materias, el semestre al que pertenecen y sus créditos.
- Nombres Argentina:Lista de nombres 
- Apellidos Argentina: Lista de apellidos 

Estos datos se cargan desde archivos CSV alojados en GitHub.

 3. Transformación de Datos de Materias
Se procesa la información de créditos de las materias para generar dos columnas adicionales:
- HTD 
- HTI
Además, se genera un código único para cada asignatura basado en su nombre.

 4. Generación de Nombres Completos
Utilizando las listas de nombres y apellidos, se crean combinaciones de nombres completos (nombre + primer apellido + segundo apellido) para simular una lista de estudiantes.
 
5. Clasificación de Materias por Semestre
Se organiza la lista de materias por semestres. Para cada semestre, se agrupan las materias correspondientes en listas separadas.

 6. Creación de Directorios y Archivos
Para cada materia en cada semestre:
1. Se crea una estructura de directorios siguiendo el formato R/Semestre X/Materia.
2. Dentro de cada directorio de materia, se generan dos archivos:
   - Un archivo CSV.
   - Un archivo Excel.
   
Los nombres de los archivos siguen un formato que incluye un código de curso, el nombre de la materia, un identificador de semestre y una letra d.

 7. Estructura Final
El resultado es una jerarquía de carpetas donde cada carpeta de semestre contiene subcarpetas para cada materia. Dentro de estas subcarpetas, se encuentran los archivos CSV y Excel con los nombres de los estudiantes matriculados en cada materia.
 

