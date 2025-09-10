# Practica2-Dashboard
Ingresar datos en tiempo real desde OpenWeatherMap mostrandolos en un dashboard de la terminal usando una instancia de AWS EC2 con Ubuntu.

---
## 1. Actualización e instalación de recursos

Actualizamos los datos del sistema con el siguiente código:
```bash
sudo apt update
```
Posteriormente, con el siguiente comando verificamos si estan correctamente instalados python y pip
```bash
sudo install python3 python3-pip python3-venv -y
```
Luego, se ingresa el siguiente comando para instalar dashing
```bash
pip install dashing
```

## 2. Entorno virtual
Al estar trabajando en una terminal virtual, se debe de ingresar el siguiente código para evitar errores a la hora de ejecutar los comandos proximos:
```bash
python3 -m venv dashing-env
source dashing-env/bin/activate
```
Por último, instalamos una dependencia
```bash
pip install urwid requests
```

## 3. Creación del scrip
Ahora, se ejecuta el siguiente comando:
```bash
nano clima.py
```
Se abrira una pestaña donde ingresaremos el código que se nos proporciono anteriormente, con la combinación de las teclas "ctrl + o" para guardar la información y "ctrl + x" para salir del archivo.
<img width="1369" height="552" alt="imagen" src="https://github.com/user-attachments/assets/33a203d6-3e17-43ff-a05f-91357cb89d87" />

En la página de "OpenWeather" en la sección de "Api Keys" copiamos la llave que se nos genera automaticamente:
<img width="1911" height="457" alt="imagen" src="https://github.com/user-attachments/assets/c2b94a78-0a7a-4999-8f3b-b03281e473e1" />

## 4. Ejecución del Dashboard
Finalmente, con el siguiente comando se muestra en la terminal el dashboard
```bash
python3 clima.py
```

## 5. Video de Asciinema
Se anexa el video grabado con Asciinema lo que se documento anteriormente:
[![asciicast](https://asciinema.org/a/CP07D4MQDt3AvaZ855SN02KRO.svg)](https://asciinema.org/a/CP07D4MQDt3AvaZ855SN02KRO)
