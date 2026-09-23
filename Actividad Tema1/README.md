#Actividad Tema 1: Como desarrollar un juego o pequeña app.

Vamos a desarrollar un juego Roguelike.

ETAPA 1:PROBLEMA, PLATAFORMA Y LENGUAJE ELEGIDO.

Para este caso elegiremos java como lenguaje para su desarrollo.

Como plataforma elegiré pc, ya que es la mas conocida (mayor alcance) y ofrece buen soporte para desarrolladores.

ETAPA 2: ALGORITMO O EJEMPLO DE PARADIGMA QUE USARÍAS.


Creamos diferentes elementos a partir de funciones con objetos enlazados entre sí para crear esa interconexión que permitirá ejecutar el juego y que todos los elementos tengan sentido.
Los elementos estarán estructurados de forma independiente para que sea facil identificar cada uno en el código.


Estructura básica del diseño:

Personajes: Protagonista controlado por el jugador y secundarios (que acompañen o no al jugador).
Enemigos: Elementos dañinos para el jugador así como para personajes secundarios.
Equipamiento: Aquí añadiremos diferentes ramas clasificadas segun el tipo. Tipo de armas, armaduras, objetos especiales.
Entorno/Mapas: Desarrollamos una serie de mapas con diferentes efectos únicos (tormentas de rayos, tornados, etc...)

Ahora vamos con los sitemas que unen estos elementos:

Los elementos como personajes y enemigos tendrán un sistema de vida basado en una barra de salud que ira disminuyendo conforme sufran cualquier tipo de daño.

Elementos como el equipamiento tendrá un sistema similar basado en durabilidad, es decir, cuando mas sea usado menos durabilidad tiene.
A esto le añadiremos un sistema de reparación con el que podremos recuperar la durabilidad del equipamiento.

Ahora añadiremos un sistema de rarezas tanto para enemigos como para equipo.
La base es la misma apra ambos elementos pero se desarrollará de forma diferente. Para el equipo usaremos un sistema básico de colores para clasificar su rareza (ej: blanco=común, azul=raro, etc...) mientras que para los enemigos usaremos este mismo sistema de colores pero con una clasificación diferente (ej:blanco=normal, azul=élite, etc...). 
Ambos sistemas seguiran una serie de reglas aplicadas a cada elemento para generar una serie de características únicas segun la rareza del mismo (ej: arma azul=mayor número de estadisticas, arma dorada=habilidad única, enemigo, etc...).

Dado que es un roguelike, el juego debe tener un sistema de rejugabilidad, asi que añadiremos un sistema de muerte semi-permanente donde perderemos el equipo que vamos consiguiendo a lo largo de los diferentes mapas. A cambio, obtendremos una moneda especial para desbloquear un sistema de habilidades que te den estadisticas permanentes, así como habilidades únicas (ej: Al morir puedes elegir una pieza de equipo para quedarte con ella de forma permanente. Puedes contratar acompañantes que te ayuden durante los diferentes mapas. etc...)

Ahora revisaremos el diseño, utilizaremos un estilo oscuro estilo diablo, con diseños detallados de los elementos (personajes, enemigos, equipamiento, mapas), el juego estará desarrollado en vista aérea.

Añadiremos un campamento donde el jugador estará cada vez que muera en la partida.
Aquí habrá elementos como la hoguera y el cofre donde almacenaremos el equipamiento así como otros objetos. Añadiremos un sistema de subida de nivel para ambos objetos, que ofrecerán ventajas como mayor hueco de almacenamiento (cofre) o ventajas extras para la siguiente partida (hoguera).

ETAPA 3: CÓMO LLEGA EL CÓDIGO A EJECUTARSE.

Para su ejecución usaremos un ejecutable (.exe). 
Al iniciarlo aparecera el menu con un botón que tendrá la función "iniciar partida", al pulsarse comenzará el juego.






