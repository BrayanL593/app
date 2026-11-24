NETQUEST VR/AR — APLICACIÓN WEB INTERACTIVA

Incluye:
- Inicio y navegación entre módulos.
- Cuatro lecciones completas sobre redes y modelo OSI.
- Quiz de 10 preguntas, respuestas, corrección y puntuación.
- Explorador de dispositivos con fichas educativas y activación opcional de cámara.
- Simulación de centro de datos con tres retos interactivos.
- Perfil con nombre editable, puntos, insignias y progreso.
- Guardado local automático mediante localStorage.
- Diseño adaptable a escritorio, tablet y celular.

EJECUCIÓN:
1. Descomprime el ZIP.
2. Abre index.html en un navegador moderno.

CÁMARA:
Por seguridad, el acceso a cámara requiere HTTPS o localhost. Para probar cámara localmente, puedes abrir una terminal dentro de la carpeta y ejecutar:
  python -m http.server 8000
Luego visita http://localhost:8000

NOTA:
La RA es una experiencia de demostración con cámara y ficha del dispositivo; no incluye reconocimiento automático de marcadores ni tracking 3D real. La RV es una simulación interactiva en navegador, no requiere visor VR.
El progreso se guarda en el navegador actual y no se sincroniza entre dispositivos.

CORRECCIONES DE LA VERSIÓN REVISADA:
1. Reto 2 (direcciones IP): la validación rechazaba toda dirección por un doble escape
   en la expresión regular. Ahora acepta direcciones IPv4 privadas válidas y rechaza
   valores fuera de rango.
2. Pie de página: la etiqueta <footer> no tenía la clase declarada en la hoja de
   estilos, por lo que se superponía al contenido. Corregido.
3. Quiz: al volver a entrar al módulo se conservaba el intento anterior. Ahora el
   cuestionario se reinicia al abrir el módulo.
