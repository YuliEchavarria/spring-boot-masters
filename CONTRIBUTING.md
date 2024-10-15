# Contributing para Estramipime Backend
Gracias por tu interés en contribuir a este proyecto. A continuación se detallan las directrices que deben seguirse para proponer cambios, así como el proceso de revisión e integración de los mismos.

## Requisitos para Contribuir
1. Crea una rama basada en el ticket correspondiente de Jira:

* El nombre de la rama debe ser exactamente el mismo que el generado en Jira para la tarea o ticket.
* Ejemplo: Si el ticket en Jira tiene el identificador SP-123, entonces tu rama debe llamarse `SP-123-descripción-de-tu-tarea`.
2. Realiza los cambios en tu rama.

3. Antes de proponer un **Pull Request**:

* Asegúrate de que tu rama esté actualizada con la rama `master`. Si no es así, realiza un rebase sobre la rama master y aplica los cambios necesarios.
```
git checkout master
git pull origin master
git checkout SP-123-descripción-de-tu-tarea
git rebase master
```
4. Verifica que tus cambios pasen las pruebas y linters correspondientes.

## Creación de un Pull Request
1. Crea un Pull Request:

* Asegúrate de que el título y la descripción del Pull Request estén claros y que mencionen el número del ticket de Jira.
* El Pull Request debe estar dirigido a la rama main.
2. Revisión:

* El Pull Request debe ser aprobado por al menos dos revisores antes de ser integrado a la rama main.
* Responde a los comentarios de los revisores y realiza los cambios necesarios.
3. Merge:

* Solo una vez que al menos dos personas hayan aprobado el Pull Request, se podrá hacer el merge a main.
El merge debe realizarse en base a la última versión de master.
  ## Rebase
Si tu rama no está basada en la última versión de master, debes realizar un rebase antes de solicitar la integración del Pull Request. Esto garantiza que todos los cambios estén alineados con la versión más reciente del proyecto.

Para realizar un rebase:

```
Copiar código
git checkout master
git pull origin master
git checkout SP-123-descripción-de-tu-tarea
git rebase master
```
Resuelve cualquier conflicto que aparezca durante el rebase, verifica los cambios, y continúa con el proceso de commit y push.

### Proceso de Contribución Resumido
1. Crea una rama basada en el ticket de Jira.
2. Realiza un rebase para asegurar que tu rama esté alineada con master.
3. Crea un Pull Request que debe ser aprobado por dos revisores.
4. Si es necesario, realiza un rebase adicional para integrar la rama a main.
5. Después de la aprobación, integra la rama a main.
