# Pasos para Modificar el Archivo `backend.js` en el Servidor

Este archivo proporciona una guía paso a paso para modificar el archivo `backend.js` en el servidor y recrear el proceso correspondiente con PM2. Sigue los pasos a continuación para realizar correctamente las modificaciones.

---

## 1. Acceder a Google Cloud Console
Accede al panel de control de Google Cloud para gestionar las máquinas virtuales y los servicios en la nube.

- Ir a: [Google Cloud Console](https://console.cloud.google.com/)
- Iniciar sesión con tu cuenta personal.

## 2. Entrar en Compute Engine
Una vez dentro de la consola de Google Cloud:

- Navega a **Compute Engine > Instancias de VM**.

## 3. Seleccionar la VM `familyseriestrackbackend`
Encuentra la instancia llamada `familyseriestrackbackend` y selecciónala para gestionar su configuración y archivos.

## 4. Abrir la conexión SSH
Abre una conexión SSH con la VM para acceder al sistema de archivos y gestionar el backend:

- Haz clic en el botón **SSH** y espera a que se inicie la sesión en la terminal.

## 5. Eliminar el archivo `backend.js` 
- Dentro de la sesión SSH, elimina el archivo `backend.js` existente:

``` 
sudo rm -rf backend.js
```

 ## 6.  Subir el nuevo archivo `backend.js`
- Se utiliza la propia interfaz de google

 ## 7.  Reiniciar el proceso con PM2
- Utilizando el comando:
```
pm2 restart backend
```

 ## 8.  Verificar que el servidor está funcionando
- Verifica el estado del proceso con el comando:
```
pm2 status
```










Este `README.md` está estructurado con títulos claros, código correctamente formateado, y un flujo sencillo para que cualquier persona pueda seguir los pasos fácilmente. ¡Espero que te guste el formato! Si necesitas alguna modificación, avísame.
