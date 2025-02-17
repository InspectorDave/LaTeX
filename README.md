# Repositorio para apuntes, guías y documentos para dar clases

Este repositorio es para recopilar apuntes, guías y documentos que utilicé para dar clases, ya sea como profesor particular o ayudante de la materia Redes en FIUBA. Fueron hechos por mí para asistirme en la enseñanza. No buscan estar completos, ser exhaustivos y pueden llegar a tener errores. Si encontrás alguno por favor hacémelo saber.

Junto con los documentos están los archivos LaTeX que los generan y las imágenes que utilizan.

# Sobre el autor

Soy Ezequiel Mundani Vegega, actualmente estoy estudiando Ingeniería Informática en la UBA y antes estudiaba Ingeniería Electrónica. El secundario lo hice en el Colegio Nacional de Buenos Aires.

Doy clases particulares desde 2020, principalmente de matemática, física, química; y desde 2024 soy ayudante en la materia Redes de FIUBA.

En caso que quieras contactarme, este es mi mail: emundani@fi.uba.ar

# Si los querés usar

Podés utilizarlos y compartirlos, pero en caso de modificarlos o editarlos tendrás que citar al autor.

# Cómo utilizar LaTeX

Hay varias maneras de utilizar LaTeX, la más fácil es Overleaf (https://www.overleaf.com/) si lo querés usar en la nube, pero es lento y con el tiempo te quitan funcionalidades a menos que les pagues. Tiene un máximo de 2 editores por proyecto (creador + 1). Personalmente uso TeX Live integrado con VS Code.

## Cómo utilizarlo localmente

- Instalar TeX Live desde su página web: https://www.tug.org/texlive/
    - Recomiendo descargar el ISO con un torrent https://www.tug.org/texlive/acquire-iso.html (25 minutos de descarga + 20 minutos de instalación) en vez de la descarga "fácil" (10 horas de descarga + 20 minutos instalación).
    - En Windows:
        - Correr el .exe que está dentro del .iso 
    - En Unix:
        - Ir dentro de la imagen .iso
        - Correr `sudo perl ./install-tl --no-interaction`
        - Al finalizar la instalación, te va a decir que agregas el directorio donde lo instalaste a $PATH:  en el directorio home.
            - Ir al directorio home
            - Abrir como root .bashrc
            - Al final de archivo poner `export PATH="/usr/local/texlive/2024/bin/x86_64-linux/latexmk:$PATH"`, reemplazando por la ubicación de latexmk
        - Cerrá sesión y volvete a logear
        - Verificá que se haya instalado correctamente corriendo `which latexmk`
- Instalar VSCode
- En VSCode, instalar la extensión de LaTeX Workshop (la de James Yu)
- Ya estás en condiciones de usar LaTeX de manera local. Arriba a la derecha está la flechita verde para compilar.
- Es una buena idea tener tu proyecto en un repo de GitHub, de esta manera podés colaborar con todos los que quieras y mientras una persona cambia algo no te "rompe" la compilación a vos.
- Recomendaciones desde VSCode:
    - Instalá un corrector de ortografía (por ejemplo, Spell Right de Bartosz Antosik).
        - Desde configuración, que te marque los errores como info en vez de error.
    - Deshabilitá la compilación automática desde VSCode y asignale una hotkey (yo uso ctrl+shift+R).
    - Establecé un output directory (yo utilizo Output) y agregalo a .gitignore.
    - Con ctrl+click en el .pdf vas al código que lo genera.
