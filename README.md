# Actividad
## 1. Inicio del script
![[img1.png]]
## 2. Agregar un submódulo
![[img2.png]]
## 3. Gestión de ramas
![[img3.png]]
## 4. Gestión de git diff
![[img4.png]]
## 5. Gestión de hooks
![[img5.png]]
# Preguntas

### 1. ¿Qué diferencias observas en el historial del repositorio después de restaurar un commit mediante reflog?

### 2. ¿Cuáles son las ventajas y desventajas de utilizar submódulos en comparación con subtrees?
Los submódulos permiten vincular un repositorio externo como dependencia, manteniéndolo separado del repositorio principal, facilitando mantener actualizaciones independientes. Aunque puede ser complicado de usar porque se requiere de comandos específicos para clonar, actualizar o hacer commits. Los subtrees integran el repositorio externo dentro del historial del proyecto principal, simplificando la gestión para usuarios. Dificultando mantener sincronización con el repositorio original al hacer cambios muy frecuentes.
### 3. ¿Cómo impacta la creación y gestión de hooks en el flujo de trabajo y la calidad del código?
Los hooks permiten ejecutar scripts automáticamente en distintos momentos del ciclo de vida de los commits, como antes de hacer un commit o un push. Mejorando  la calidad del código gracias a las verificaciones automáticas como pruebas unitarias o validación de mensajes de commit. Aunque su mantenimiento puede ser un desafío en equipos grandes si no se gestionan bien, ya que no se versionan por defecto con el repositorio.
### 4. ¿De qué manera el uso de `git bisect` puede acelerar la localización de un error introducido recientemente?
git bisect automatiza la búsqueda binaria en el historial de commits para encontrar el punto exacto donde se introdujo un error. En vez de revisar todos los commits uno a uno, permite dividir el rango de commits en mitades y verificar si el error aún está presente, reduciendo drásticamente el número de pruebas necesarias. 
### 5. ¿Qué desafíos podrías enfrentar al administrar ramas y stashes en un proyecto con múltiples colaboradores?

# Ejercicios

## 1. Funcionalidad para renombrar ramas
### Modificar la función de "Gestión de ramas"
![[img6.png]]
### Implementación:
![[img7.png]]
### Verificación:
![[img8.png]]
## 2. Diferencias de un archivo entre 2 commits o ramas
### Creación *main.py* con cambios hechos solo en master:
![[img9.png]]
### Creación de la función Comparar diferencias de un archivo específico:
![[img10.png]]
### Validación:
![[img11.png]]
## 3. Funcionalidad para instalar un hook
### Creación del hook *pre-commit*:
![[img12.png]]
### Integración del hook en *git_avanzado*:
![[img13.png]]
### Validación:
![[img14.png]]
![[img15.png]]
## 4.  Merge automatizado de una rama
### Creación y validación:
![[img16.png]]
## 5. Reporte con información relevante del repositorio
