# Objetos
- Noticia
  - Título
  - URL
  - Reseña
  - Fuente
  - Tags
  - Imagen
  - Fecha de publicación
  - Fecha de adquisición (`created_at`)
  - Fecha actualización

- Comentario
  - Usuario
  - Contenido
  - Valoración
  - Fecha de publicación

- Fuente de noticia
  - Nombre
  - Logo
  - Imagen
  - URL

- Usuario
  - Nombre
  - Correo
  - Preferencias/Gustos

# Formato de comunicación:
- JSON
- Métodos GET/POST a la URI del componente.

Puertos de Comunicación entre Componentes

# Sobre los componentes
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
