# SSBash

SSBash es un escript en Bash para crear aplicaciones web SSB (Site-specific Browser) basadas en un navegador con motor Chromim que lo soporte.

Lo que hace es, tras pedir unos datos, crear un archivo .desktop con el ejecutable necesario para que la aplicación se abra aislada y en su propio perfil.

Para lanzarlo, antes hay que darle permiso de ejecución con `chmod +x SSBash` y luego se puede lanzar con `bash SSBash` o `./SSBash`.

## Navegadores soportados

SSBash soporta:

* Chrome.
* Chromium, normal y ungoogled (ambos se lanzan con `chromium`).
* Brave.
* Edge.
* Vivaldi.
* Versiones flatpak de todo lo anterior.

## Posibles problemas

Es posible que haya poblemas al añadir la imagen o al moverla a la carpeta de configuración, lo que es menos probable si se introduce la ruta del icono manualmente. El archivo .desktop se suele crear siempre, y si falla con la imagen o al mover el acceso directo, se puede comprobar que esté todo correcto en el .desktop, moverlo manualmente a `~/.local/share/applications` y mover la imagen a la carpeta `img` de `~/.config/SSBash/nombre-de-la-app/img`.
