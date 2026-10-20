# Jardín de Bolsillo
Juego original de estrategia por turnos para Un juego cada día. Cuatro huertos, nueve parcelas, tres cultivos, lluvia previsible y tres acciones diarias. La planificación de recursos y cosechas no repite las mecánicas de Órbita de Rescate ni Faro de Medianoche.

Sin dependencias, red de juego, cuentas ni servicios externos. Todo el progreso queda en localStorage, clave `daily-games:jardin-de-bolsillo:v1`, compatible con el resumen del catálogo. No se sincroniza entre dispositivos. Guardado bloqueado se comunica en pantalla.

## Ejecutar y comprobar
`npm start` sirve en http://localhost:8080. `npm run check` valida sintaxis y pruebas de motor/almacenamiento. No requiere instalar paquetes.

## Controles y reglas
Ratón, táctil o Tab/Enter. Selecciona cultivo, regadera o cesta y una parcela. Cada acción gasta una de tres acciones diarias. Agua +2 cada mañana, máximo9. Regar añade un crecimiento, una vez por planta y día. La lluvia crece todas las plantas al terminar el día. Cosechar recupera una semilla y suma puntos; primera variedad +2. Los récords desbloquean huertos. Puedes deshacer hasta40 acciones de la sesión, conservando récords. Reiniciar/cambiar huerto sin terminar requiere confirmación. La última lluvia no cosecha automáticamente: recoge antes de acabar la temporada.

## Publicación
Repositorio independiente `mitchell-castillo/jardin-de-bolsillo`. GitHub Pages desde main, raíz. Añadir al catálogo solo tras verificar despliegue y CI. Rutas relativas compatibles con subdirectorio. SVG original creado para este juego. Sin fuentes ni assets externos.
