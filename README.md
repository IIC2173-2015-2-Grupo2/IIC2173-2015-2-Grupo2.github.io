# Proyecto

* Arquitectura del sistema en general: [architecture.pdf](architecture.pdf)
* Avance presentado: [avance.pdf](avance.pdf)

# Información

Para mantener el estandar, orden y homogeneidad:

* Programar en inglés y respetando la guía de estilo del lenguaje/framwork.
* Hacer commits limpos y claros.
	* Buen commit: `git commit -m "Agregada opción para borrar noticias viejas"`.
	* Mal commit: `git commit -m "final"`, `git commit -m "fix"`.
* Evitar `git add --all` o similares a menos que de verdad estemos seguro de lo que vamos a commitear.
* Pueden usar aplicaciones como la de Github para tener más control de lo que subimos en cada commit.
* Para evitar el típico merge que sucede cuando hacemos pull y habían cambios en la nube que no teníamos se recomienda:
  * Tener los commits listos con todos nuestros cambios.
  * Hacer `git pull --rebase`, esto se guarda los commits locales al bolsillo, baja los que estén en la nube y pone los nuestos encima de la última versión bajada.
  * Ahora sí hacemos `git push`.

## Formato de comunicación:
- JSON
- Métodos GET/POST a la URI del componente.

Puertos de Comunicación entre Componentes

## Sobre los componentes
Cada componente separado en un repositorio. Estos deben tener:
- .gitignore
- README.md
  - Información
  - Quienes trabajaron en qué entrega
  - Documentación.
    - Uso de la API
    - Documentación interna de los métodos, clases, etc.
    - Instrucciones de cómo hacer el deployment y trabajar localmente (development).
    - Declarar guía de estilo a usar. Sugerencias de IDEs, plugins, linters, etc.

- Usar las Issues para llevar track del progreso, errores encontrados, features pendientes.
- Trabajar con branches:
  - Todo repo tiene la branch master
  - De master sale la branch development.
  - La implementación de las features se desprenden de esta, una vez listas se hacen merge de vuelta a development. Idealmente hacer git squash para aplastar todos los commits dentro de esa implementación en uno.
  - Cuando development esté estable, se hace merge a master.
