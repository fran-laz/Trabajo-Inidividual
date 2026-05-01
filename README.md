# Trabajo-Inidividual
# Clase 1
  # Que es git
    Git es una plataforma para trabajar y compartir codigo de manera sencilla para trabajos en grupo
    
---

# CLase 2
  # Estados de Git

  * ## Directorio de trabajo (Modificado)
	  Es tu carpeta local donde escribes código que Git aún no ha "asegurado".

  * ## Stage Area (Preparado)
	  Es el área de espera donde seleccionas qué cambios quieres guardar.

  * ## Repositorio Local (Confirmado)
	  Es el historial donde tus cambios reciben un hash y empiezan a formar parte del proyecto.

---

  # Buenas prácticas

  * ## Commit atómico
	  Un commit atómico representa un único cambio lógico, pequeño y completo.

  * ## Hacer commits a menudo
	  Es preferible realizar commits pequeños con mejoras puntuales que uno masivo con múltiples cambios		   
	  mezclados.

  * ## Iteraciones con significado
	  Cada commit debe tener sentido por sí mismo y, preferiblemente, no dejar el proyecto sin funcionar.

  * ## Evitar commits sin sentido
	  Grabar el progreso no justifica crear mensajes o cambios aleatorios.
   ## GitHub y SSH

   GitHub es una plataforma para almacenar y colaborar en proyectos usando Git. Se recomienda usar **SSH** para conectarse, ya que evita ingresar credenciales cada vez. :contentReference[oaicite:0]{index=0}

   ## Comandos básicos

	- `git clone`: copiar un repositorio  
	- `git push`: subir cambios  
	- `git pull`: bajar cambios  
* ## Ramas y Gitflow

	Las ramas en Git permiten trabajar en diferentes partes del proyecto sin afectar el código principal. Gitflow es un flujo de trabajo que organiza el desarrollo usando ramas específicas para cada tipo de tarea,
	facilitando el trabajo en equipo y el control de versiones.

	Las ramas principales son:
		- **main**: contiene el código en producción  
		- **develop**: contiene el código en desarrollo  
		- **feature**: nuevas funcionalidades  
		- **release**: preparación de nuevas versiones  
		- **hotfix**: corrección de errores urgentes  

* ## Comandos básicos de ramas

		- `git branch`: listar o crear ramas  
		- `git branch -D <rama>`: eliminar una rama  
		- `git checkout <rama>`: cambiar de rama  
		- `git checkout -b <rama>`: crear y cambiar de rama  
		- `git switch <rama>`: cambiar de rama (comando moderno)  
* ## Comandos clave

	- **git merge**: fusiona ramas (`--no-ff` mantiene historial)  
	- **git fetch**: revisa cambios remotos sin aplicarlos  
	- **git pull**: trae y aplica cambios → `git pull origin <rama>`  
	- **git push**: sube cambios → `git push origin <rama>` (`-u` la primera vez)  


* ## Flujo básico

	1. Actualizar `develop`: `fetch` + `pull`  
	2. Trabajar en tu rama y subir cambios (`push`)  
	3. Volver a `develop`, actualizar y hacer `merge --no-ff`  
	4. Resolver conflictos, commit y eliminar la rama

* ## Pull Requests (PR)

	Los **Pull Requests (PR)** son la forma profesional de integrar cambios en GitHub. Permiten proponer la fusión de una rama al código principal, facilitando la revisión, discusión y aprobación antes del merge. 
	Se usan principalmente para mejorar la seguridad y el trabajo en equipo, evitando cambios directos sin revisión.

* ## Flujo con PR

	1. Actualizar `develop`: `fetch` + `pull`  
	2. Crear/cambiar a tu rama y trabajar  
	3. Subir cambios: `git push origin <rama>`  
	4. Actualizar tu rama con `develop` si es necesario  
	5. Crear el Pull Request en GitHub para revisión y merge   
