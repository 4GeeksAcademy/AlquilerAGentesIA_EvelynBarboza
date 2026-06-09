# AgentHub

## Descripción del producto

AgentHub es una plataforma SaaS que permite a empresas alquilar agentes de IA especializados para tareas de negocio. Los administradores gestionan usuarios, agentes, skills, contratos y monitorean el estado operativo de la plataforma.

## Stack tecnológico y restricciones

- HTML5 semántico.
- Tailwind CSS vía CDN.
- JavaScript Vanilla.
- Sin frameworks.
- Sin backend.
- Mobile First.
- Responsive.
- Datos hardcodeados.
- Considerar SEO, GEO y accesibilidad.

## Dashboard

1. Mostrar cuatro tarjetas de métricas en una cuadrícula responsive 2x2.
2. Las métricas serán: ingresos totales del mes, pérdidas por descuentos y cupones, agentes activos y agentes en estado de fallo.
3. Cada tarjeta debe incluir un icono, una etiqueta descriptiva y un valor hardcodeado.
4. Cada tipo de métrica utilizará un color de acento diferente para facilitar la identificación visual.
5. Las tarjetas tendrán una sombra suave para destacarse del fondo.
6. Debajo de las métricas se mostrará un área de placeholder para representar un gráfico de actividad semanal.

## Gestión de usuarios

1. Mostrar una tabla con todos los usuarios registrados.
2. Cada fila deberá incluir nombre, email, plan contratado y estado.
3. Cada usuario tendrá un menú desplegable de acciones accesible mediante un botón de tres puntos (⋮).
4. El menú desplegable incluirá las acciones "Ver detalle" y "Eliminar".
5. La acción "Ver detalle" abrirá un modal overlay con toda la información del usuario.
6. El modal podrá cerrarse mediante un botón de cierre o haciendo clic sobre el backdrop.
7. Los botones y acciones interactivas tendrán efectos hover.
8. La sección utilizará la misma paleta de colores definida para el Dashboard.

## Gestión de agentes

1. Mostrar un listado de todos los agentes registrados en la plataforma.
2. Cada agente mostrará nombre, propietario y estado actual.
3. Los estados posibles serán activo, inactivo y fallando.
4. Las skills asociadas a cada agente estarán ocultas por defecto.
5. Un control expandible permitirá mostrar u ocultar las skills mediante una transición suave.
6. Cada skill mostrará un tooltip descriptivo al pasar el cursor sobre ella.
7. La descripción del tooltip no superará los 50 caracteres.
8. Cada agente incluirá un menú desplegable de acciones.
9. El menú incluirá las opciones "Configurar" y "Eliminar".
10. La acción "Configurar" abrirá un modal mostrando el prompt de sistema del agente.

## Skills

1. Mostrar un catálogo de todas las skills disponibles en la plataforma.
2. Cada skill mostrará nombre, descripción breve y cantidad de agentes que la utilizan.
3. Incluir una explicación introductoria sobre el concepto de skill dentro de AgentHub.
4. Cada skill dispondrá de un menú desplegable de acciones.
5. Las acciones disponibles serán "Ver detalle" y "Eliminar".
6. La información deberá mostrarse mediante tarjetas reutilizables consistentes con el resto del diseño.
7. La sección utilizará la misma paleta visual aplicada en toda la aplicación.

## Contrataciones de agentes

1. Mostrar una tabla con contratos activos e históricos.
2. Cada fila incluirá cliente, agente contratado, skills contratadas, fechas del contrato e importe total pagado.
3. Cada contrato dispondrá de un menú desplegable de acciones.
4. La acción "Ver detalle" abrirá un modal overlay.
5. El modal mostrará información completa del contrato.
6. El detalle incluirá un desglose individual de las skills contratadas.
7. Cada skill mostrará su precio individual dentro del contrato.
8. El modal podrá cerrarse mediante botón o clic sobre el backdrop.

## Log de errores

1. Mostrar un registro cronológico de errores de ejecución de agentes.
2. Cada entrada incluirá timestamp, nombre del agente, tipo de error y descripción breve.
3. Los errores se categorizarán visualmente mediante badges.
4. Los badges utilizarán colores distintos según gravedad o tipo de error.
5. Cada registro incluirá un menú desplegable de acciones.
6. Las acciones disponibles serán "Ver detalle" y "Marcar como resuelto".
7. La acción "Ver detalle" abrirá un modal con la traza completa del error.
8. La acción "Marcar como resuelto" actualizará visualmente el estado del registro.

--------------------------------------------------------------------------------------------

Debe ser para una plataforma Saas, en la que las empresas puedan alquilar agente de IA, que puedan equiparse con distintas skills y desplegarse para distintas tareas de negocio epecificas. El panel debe incluir las siguientes seis secciones, accesibles desde una navegación lateral persistente. Un toggle en la barra superior debe permitir cambiar toda la interfaz entre modo claro y modo oscuro usando las utilidades dark: de Tailwind.

Requisitos del Panel de Administración — AgentHub
El panel debe incluir las siguientes seis secciones, accesibles desde una navegación lateral persistente. Un toggle en la barra superior debe permitir cambiar toda la interfaz entre modo claro y modo oscuro usando las utilidades dark: de Tailwind.

1. Dashboard De un vistazo, el administrador debe poder ver: ingresos totales generados (este mes), pérdida total por descuentos y cupones, número de agentes activos en todos los clientes, y número de agentes actualmente marcados como fallando. Cada uno de estos debe ser una tarjeta de métrica visible. Debajo de las tarjetas, incluye un área de marcador de posición para un gráfico de actividad semanal.

2. Gestión de usuarios Una tabla que lista todos los usuarios registrados (nombre, email, plan, estado). Cada fila debe tener un dropdown de acciones — un pequeño menú activado con un botón ⋮ — con al menos dos opciones: "Ver detalle" y "Eliminar". Al elegir "Ver detalle" se abre un modal overlay con el registro completo del usuario. El modal debe cerrarse mediante un botón y haciendo clic en el backdrop.

3. Gestión de agentes Un listado de todos los agentes registrados en la plataforma, mostrando nombre del agente, propietario, estado actual (activo / inactivo / fallando) y una lista de skills colapsada. Las skills asociadas a cada agente están ocultas por defecto; hacer clic en un control expandible las revela con una transición suave. Cada agente también tiene un dropdown de acciones con las opciones "Configurar" — que abre un modal con el prompt de sistema del agente — y "Eliminar".

4. Skills Una sección dedicada al catálogo de skills disponibles — las capacidades que se pueden adjuntar a los agentes. Cada skill tiene un nombre, una descripción breve, y un indicador de cuántos agentes la tienen habilitada actualmente. Incluye una breve explicación dentro del panel sobre qué significa una "skill" en el contexto de AgentHub. Las skills también tienen un dropdown de acciones con "Ver detalle" y "Eliminar".

5. Contrataciones de agentes Una tabla que muestra todos los contratos de alquiler activos y pasados. Cada fila debe mostrar el cliente, el agente alquilado, las skills contratadas, las fechas del contrato y el importe total pagado. Cada fila tiene un dropdown de acciones. Al elegir "Ver detalle" se abre un modal con el desglose completo del contrato, incluyendo la lista desglosada de skills contratadas y sus precios individuales.

6. Log de errores Un registro de errores de ejecución de los agentes — mostrando timestamp, nombre del agente, tipo de error y una descripción breve. Los errores deben categorizarse visualmente por tipo o gravedad usando badges con código de color. Cada entrada tiene un dropdown de acciones con "Ver detalle" (abre un modal con la traza completa del error) y "Marcar como resuelto".