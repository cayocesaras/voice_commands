# Voice commands (command your PC with spoken commands) #

You can modify the commands below to better use in the file: ~/.voice_commands/"v-c LANGS"/commands-es

The function of this program starts running play_stop.sh script, which will start recording your voice, and if after five seconds, or run it again, start voice recognition, for now, make one of all commands available.
Also can repeat the last command with RETRY function, and apply a new action with the function: ADD_NEW_ACTION
Orders can be just a simple context: << order >> , or double context: << order >> << cited-text >>
Available commands are 95

After installed we can launch it from Applications, Universal Access, Voice Commands
And you can drag and drop on the gnome panel, and to call it a keyboard shortcut, eg. F6, this is the command:
# Changing $USER, to your user name: /home/$USER/.voice_commands/play_stop.sh
First install the command line file, typing this:
sudo cp ~/.voice_commands/v-c /usr/bin && sudo cp ~/.voice_commands/v-c /usr/bin/voice-commands
# Changing $USER, to your user name: /home/$USER/.voice_commands/play_stop.sh
First install the command line file, typing this:
sudo cp ~/.voice_commands/v-c /usr/bin && sudo cp ~/.voice_commands/v-c /usr/bin/voice-commands 

v-c
or,
voice-commands

------------------------------------------------------------

#	##	v-c , command line options	##	#

v-c -r		Run
v-c -l -lang	To select another, of 67 languages, on the commands:
		 ( « -run », « -try », « -modify », « -update » and « -h » ).
v-c -t -try	To try any command. « v-c -try "order call method" »
v-c -mic [NUM]	Set the port, to use by default [1,2,3...]. And, if [input-"1,2,3..."].
v-c -vol	Set the microphone volume that is used by default. Level max. 200.
v-c -m -mod	To modify the commands file, and the README file.
v-c -u -update	To update the README file, after modify the script.
v-c -a -add	To add, create, a new voice command action « v-c -add »,
		 or « v-c -add "action name" »,
		 or « v-c -add "action name=one call method;another call method"
		Separating between NAME and ORDER with =. And between ORDERS, with ;
v-c -tr		Translate some new action, if you not translated yet.
v-c -remove	To remove a new action, if doesn't need it any more.
v-c -v		Print the program version.
v-c -h		Show instructions README file.
v-c --help	Show this message

------------------------------------------------------------

Dependencies:
Internet access.
Active, and correct volume Microphone, Check: System Settings, Sound, Internal microphone, to Microphone.
You can modify the microphone port, of the command that activates microphone, and again to internal microphone, the default port is 1, if you have that recognition is not done, you can modify by command with:

 « v-c -mic '1, 2,...' »

 and, if is Microphone / Microphone '1, 2,...', then will be:

 « v-c -mic '1, 2,...' input-'1, 2,...' »
 « v-c -mic '1, 2,...' input-' ' » [ empty for 'reset' to no ";input-" ]

And if by errors of machine translation, has commands some misspelled or repeated, must modify also, can doit with the command:
v-c -m, or, v-c -mod
If your language uses apostrophes this (') should replace by an space this ( ), because it could cause conflicts.
In the files: 
/play_stop.sh and 
/speech_commands.sh


Install dependencies:
xdotool gnome-nettool gawk curl wget cheese audacious sox flac pulseaudio alsa-utils

Programs that use and are already in the distribution:
rhythmbox nautilus gcalctool gedit eog libreoffice-writer libreoffice-calc libreoffice-impress libreoffice-draw libreoffice-math

###### ACTIONS AVAILABLES ######

   Command name
   *activate with*

################################
   SELECT_FILE << cited-text >>
   (selecciona | seleccionar)
################################
   MUSIC_START
   (pone música | pone una música | play una música | poner una canción | reproducir una canción | poner música | reproductor de música | play música | pausar la música | pausa música | música | pausa)
################################
   MUSIC_START_SONG << cited-text >>
   (poner una música de | play una música de | poner una canción de | reproducir una canción de | poner música de | música de | reproducir a | reproducir música de | tocar música de)
################################
   MUSIC_PLAY
   (inicia la música | iniciar la música | interrumpir | detiene la música | música play | música pausa | iniciar música | parar música | detener música)
################################
   MUSIC_NEXT
   (música siguiente | canción siguiente | siguiente canción | canción próxima | próxima canción | pista siguiente | siguiente pista | pista próxima | próxima pista)
################################
   MUSIC_PREV
   (música anterior | canción previa | previa canción | canción anterior | anterior canción | pista previa | previa pista | pista anterior | anterior pista)
################################
   MUSIC_SHUFFLE
   (azar | desactiva al azar | música aleatoria | mezclar | no mezclar)
################################
   MUSIC_REPEAT
   (repetición | no repita | repita | repetir | no repetir)
################################
   MEDIA_REW
   (atrás | rebobinar | volver | atrasar | rebobinar | pasar para atrás)
################################
   MEDIA_FF
   (avanza | siga adelante | adelantar | pasar para adelante)
################################
   VOLUME_DOWN
   (reduce el volumen | menos volumen | reducir el volumen | reduzca el volumen | bajar el volumen | bajar volumen | menos volumen | volumen menos)
################################
   VOLUME_UP
   (aumenta el volumen | sube el volumen | subir el volumen | subir volumen | más volumen | volumen más)
################################
   VOLUME_MUTE
   (silencia el sonido | poner mudo | quitar mute | quitar el mute | audio activa | sin audio | sin volumen | apagar volumen | mudo)
################################
   SEARCH
   (buscar)
################################
   NO_STAND_OUT
   (quitar el resaltado | no resaltar | quita el resaltado | quitar resaltado)
################################
   TRANSLATE [from] [to] << cited-text >>
   (traducción de | traducir a | traducir desde | la traducción del | traducir el | traduce el | traducción de el | traducir del | traduce de el | traducción de el | traduce del | traducción del | traducir desde | traduce desde | traducción desde | traducir de el | traduce de el | traducción de el | traducir de | traduce de | traducción de | traducir | traduce | traducción)
################################
   WRITE
   (escríbeme | escribir | escribe | escriba)
################################
   WRITE_CAPITAL
   (capitaliza|mayúsculas | escribir con mayúscula | escribir en mayúscula)
################################
   WRITE_CAPITAL_ALL
   (escribir en mayúsculas | escribir todo en mayúscula | escribir todo con mayúscula
SAY_THIS << cited-text >>
   (di | decir esto | decir)
################################
   GOOGLE_SEARCH << cited-text >>
   (buscar en google | buscar en internet | google | busca en google | busca en internet | significado de | que es | buscar en el diccionario | busca en el diccionario)
################################
   YOUTUBE_SEARCH << cited-text >>
   (búsqueda de vídeos | vídeo | buscar el video | buscar el vídeo | buscar en youtube | que hay de | buscar videos de | videos de | buscar vídeos de | vídeos de)
################################
   WIKI_SEARCH << cited-text >>
   (buscar en wiki | buscar en la wikipedia | que hay en wiki | que hay en wikipedia | wikipedia)
################################
   WEATHER << cited-text >>
   (clima | clima en | clima de)
################################
   SEARCH_MAPS << cited-text >>
   (dónde está | mapa | muéstrame el mapa de | buscar mapa de | mapa de | donde es)
################################
   SAY_HI << cited-text >>
   (saluda | saluda a | saluda al | saluda a el)
################################
   HELLO
   (hola | hola compu)
################################
   WHOAMI
   (quien soy yo)
################################
   OPEN_FOLDER << cited-text >>
   (abrir directorio | abrir carpeta | abrir carpeta de | abrir directorio de)
################################
   SAY_TIME
   (dime la hora | que hora es | que hora son)
################################
   SAY_DATE
   (datos | cual es la fecha de hoy | que fecha es | que día es | que fecha es hoy | que día es hoy | dime la fecha | en que fecha estamos)
################################
   DICTATION << cited-text-continuo >>
   (modo dictado | salir modo dictado | terminar modo dictado)
################################
   UNDO
   (cancelar | deshacer)
################################
   REDO
   (rehacer)
################################
   DEL_LINE
   (borrar linea)
################################
   FAV
   (añadir a favoritos)
################################
   CLOSE_TERM
   (cerrar la terminal | cerrar terminal)
################################
   MAIL
   (abrir el e -mail | abri e -mail | leer el correo electrónico | leer el post | leer el e -mail | leer el correo electrónico | abrir mail | abrir email | abrir correo | mail | email)
################################
   COPY
   (copiar)
################################
   PASTE
   (pega | pegar)
################################
   CUT
   (corta | cortar)
################################
   SELECT_ALL
   (seleccionar todo)
################################
   SAVE
   (salva | guardar el archivo | guardar | guardar archivo)
################################
   SAVE_AS
   (guardar como | guardar la página como | guardar archivo como | guardar el archivo como | guardar página como)
################################
   FOLDER
   (crea la carpeta | crear carpeta | nueva carpeta)
################################
   MINIMISE
   (minimiza | minimizar)
################################
   MAXIMISE
   (maximiza | maximizar)
################################
   FULLSCREEN
   (pantalla completa)
################################
   TAB
   (lengüeta | tabula | tabular | tabulación)
################################
   ESC
   (esc | escape)
################################
   MENU
   (abre el menú principal | menú principal | abrir menú principal)
################################
   ACTIONS_MENU
   (menú | abrir menú | cerrar menú)
################################
   CLOSE
   (cerrar el programa | salir | cerrar programa | salir del programa)
################################
   CLOSE_WIN
   (cerrar ventana)
################################
   ZOOM_OUT
   (disminuir el zoom | alejar | achicar | disminuir | zoom menos)
################################
   ZOOM_IN
   (imagen más grande | zoom | acercar | agrandar | aumentar | zoom mas)
################################
   ZOOM_RESET
   (tamaño original | quitar el zoom | quitar el zoom | tamaño normal | zoom cero)
################################
   TOUCH_ON_OFF
   (deshabilitar el touchpad | activa el touchpad | apagar ratón táctil | encender ratón táctil | touchpad)
################################
   BACK
   (atrás | retroceder | volver)
################################
   ADVANCE
   (avanzar | adelante)
################################
   RIGHT
   (derecho | derecha)
################################
   LEFT
   (izquierda)
################################
   DOWN
   (abajo)
################################
   UP
   (sube | arriba)
################################
   PAGE_DOWN
   (bajar)
################################
   PAGE_UP
   (subir)
################################
   HOME_PAGE
   (parte superior de la página | volver al principio | principio de la página | ir al principio de la página | ir al principio)
################################
   END_PAGE
   (ir al final de la página | ir a la parte inferior de la página | final de la página | ir al final de la página | ir al final)
################################
   HOME
   (comienzo | principio)
################################
   END
   (fondo | final)
################################
   SCROLL_DOWN
   (desplácese hacia abajo | desplaza hacia abajo | bajar página | correr para abajo | correr hacia abajo)
################################
   SCROLL_UP
   (ejecutar en la página | desplazarse hacia arriba | subir página | correr para arriba | correr hacia arriba)
################################
   DELETE
   (borrar | elimina | borrar)
################################
   ENTER
   (abrir | ejecutar | enter)
################################
   NEW_WINDOW
   (nueva ventana | ventana nueva)
################################
   CHANGE_TAB << cited-numbers >>
   (pestaña | cambio a la pestaña | cambia a pestaña | cambia a la pestaña | mover a pestaña | ir a pestaña | cambiar a pestaña | ventana | cambio a la ventana | cambia a la ventana | cambia a ventana | mover a ventana | ir a ventana | cambiar a ventana)
################################
   CLOSE_TAB
   (cerrar pestaña)
################################
   BROWSER
   (abra el navegador | navegador | abrir navegador | internet)
################################
   FILE_MANAGER
   (nautilus | abre nautilus | abrir el explorador de archivos | gestor de archivos | abra el administrador de archivos | nautilo | explorador de archivos | abrir nautilus | abrir explorador de archivos)
################################
   TERMINAL
   (abrir la consola | abre la consola | abrir nueva consola | abre consola | abrir consola | abrir una terminal | abrir terminal | abre terminal | abrir nueva terminal | abrir la terminal | abre la terminal)
################################
   EXECUTE
   (ejecuta comando | ejecuta comando | lanzar comando | ejecutar comando)
################################
   BATTERY
   (batería | estado de la batería | carga de la batería)
################################
   TEXT_EDITOR
   (abra el editor de texto | lanza el editor de texto | editor de texto | abrir editor de texto | lanzar editor de texto | texto nuevo)
################################
   SCREENSHOT
   (pantalla | captura de pantalla | captura)
################################
   ALARM << cited-numbers [days] [hours] [minutes] [seconds] to sleep >>
   (fija la alarma | fija la alarma a | alarma | alarma a)
################################
   LOG_OFF
   (desconectar | termina la sesión | cerrar sesión | salir de la sesión)
################################
   BRIGHTNESS_UP
   (aumenta el brillo | aumentar el brillo | sube el brillo | súbele el brillo | auméntale el brillo | subir brillo | aumentar brillo)
################################
   BRIGHTNESS_DOWN
   (reduzca el brillo | reduce el brillo | reducir el brillo | bajar el brillo | disminuir el brillo | bajar brillo | disminuir brillo)
################################
   POWER_OFF
   (apagar el sistema | apagar el pc | apagar el ordenador | apagar el sistema | apagar la máquina | apagar la computadora | apagar computadora | apagar)
################################
   CALCULATOR << cited-operation >>
   (calcula | calcular | hacer la cuenta | hacer la operación | hacer el calculo | calculadora)
Sum (más | sumado | sumarle | suma | mas)
Rest (menos | restarle | restado | resta)
Multiplication (multiplicado por | multiplicarlo por | multiplicado | por | multiplicación | multiplicado entre)
Division (dividido entre | dividido en | dividido | dividir entre | sobre | división)
Square (al cuadrado | cuadrado de | elevado al cuadrado | cuadrado)
Percent (por ciento | porcentaje | por ciento de | porcentaje de | )
Root (raíz cuadrada de | raíz cuadrada | raíz)
Dot (punto)
Comma (coma)
################################
   TAKE_PICTURE
   (tomar una fotografía | cheese | comienza queso | fotografía | tomar una foto | tomar una fotografía | foto)
################################
   TAKE_VIDEO
   (registrar un vídeo | grabación de un vídeo | grabar | grabar un vídeo | grabar un video)
################################
   ADD_NEW_ACTION
   (añadir nuevo comando | crear nuevo comando | hacer nuevo comando | agregar un nuevo comando | crear un nuevo comando | hacer un nuevo comando | nuevo comando | nuevo orden | nueva acción)
################################
   OPEN_FILE
   (abrir el archivo | abrir archivo | abrir un nuevo archivo | abre el archivo | abre archivo | abre un nuevo archivo)
################################
   OFFICE << cited-text [ writer, calc, impress, draw, math ] >>
   (crea un nuevo documento | abra un nuevo documento | crea un nuevo documento | abra un nuevo documento | nuevo documento | abrir un nuevo documento de | abrir un nuevo documento | crear un nuevo documento de | crear un nuevo documento | crear un nuevo | crear una nueva | abrir un nuevo | abrir una nueva)
Writer (texto)
Calc (hoja de cálculo)
Impress (presentación | página | web)
Draw (dibujo | gráfico)
Math (fórmula | matemática)
################################
   RETRY
   (reintentar la orden | reintentar comando | repetir la orden | repetir comando | reiterar la orden | reiterar comando | reintentar | repetir | reiterar)
################################

You can find many more features available with this command:
Multimedia and Media:
# grep "XK_" /usr/include/X11/XF86keysym.h|sed 's/XK_//g' > ~/"More commands" && gedit ~/"More commands"
All the others:
# grep "XK_" /usr/include/X11/keysymdef.h|sed 's/ XK_/ /g' > ~/"Many more commands" && gedit ~/"Many more commands" 

With these you can create your own actions.
Use 'xdotool key XF86...', or 'xdotool key "Combination+of+keys "' for key functions,
and for write 'xdotool type "write whatever you want"'

If some do not have it configured, you can do it in System Settings, Keyboard, Keyboard Shortcuts. If the functions are listed as active but try and not to walk, please point the keyboard shortcut, click on the combination with established key again and it will offer New accelerator, and select the same source contained.
There are more options in Keyboard Settings distribution options. As log out, with Killing X, with (Ctrl+Alt+BackSpace).
The "+" only when you type the command doesn't when you press it, in this case do not push.

# Download others languages on Gnome-Look.org
http://gnome-look.org/content/show.php?content=165529

############# Written by Rodrigo Esteves ###############
### baitsart@gmail.com www.youtube.com/user/baitsart ###
# GNU License. You are free to modify and redistribute #


