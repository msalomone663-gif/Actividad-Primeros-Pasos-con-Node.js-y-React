Martin Salomone
Node.js y React

¿Para qué sirve el archivo package.json?
El archivo package.json nucleo de cualquier proyecto en Node.js.
contiene:
Metadatos esenciales: Nombre del proyecto, versión y descripción.
Scripts de automatización: Comandos personalizados como npm run dev para levantar el servidor o `npm run build` para compilar la app.
Gestión de dependencias: El listado exacto de las librerías externas que requiere la aplicación para funcionar (y sus versiones correspondientes). 
Gracias a esto, cualquier otro desarrollador puede descargar el repositorio vacío y reconstruir el entorno ejecutando simplemente npm install.

¿Qué diferencia notaron entre ejecutar un archivo directamente con Node.js y levantar el servidor de React?
la Ejecución directa con Node.js (`node app.js`): Es una ejecución lineal, de una sola pasada y del lado del servidor (backend / consola). Node interpreta el archivo JavaScript, ejecuta sus instrucciones de arriba a abajo en la terminal y el proceso finaliza inmediatamente al terminar la última línea. Si se realizan cambios en el código, es necesario volver a ejecutar el comando manualmente para verlos reflejados.
AL levantar el servidor de React con (`npm run dev` con Vite) se crea un entorno de desarrollo continuo y persistente que corre de fondo. No termina de inmediato, sino que se queda escuchando cambios. Además, incluye **HMR (Hot Module Replacement)**, lo que significa que procesa, compila y despliega el código automáticamente en el navegador web en tiempo real cada vez que guardamos un archivo, facilitando el desarrollo del frontend de forma interactiva.
