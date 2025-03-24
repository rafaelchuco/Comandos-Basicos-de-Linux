# **🚀 Comandos Básicos de Linux**  

<p align="center">
  <img src="https://www.artistapirata.com/wp-content/uploads/2018/12/programas-full-linux-descargar-programas-linux-300x181.jpg" 
       style="width: 500px; height: auto;">
</p>

---

## **📂 1. Gestión de Directorios y Archivos**  

### 📁 Navegación entre directorios  
| Comando | Descripción | Ejemplo |
|---------|------------|---------|
| `pwd` | Muestra la ruta del directorio actual. | `$ pwd` → `/home/rafael` |
| `cd directorio` | Entra en el directorio especificado. | `$ cd Documentos/` |
| `cd ..` | Sube un nivel en la jerarquía de directorios. | `$ cd ..` → De `/home/rafael/Documentos` a `/home/rafael` |
| `cd /ruta/completa` | Se mueve a una ruta absoluta. | `$ cd /var/www/html` |
| `cd ~` | Vuelve al directorio personal del usuario. | `$ cd ~` → `/home/rafael` |

### 📜 Listado de archivos  
| Comando | Descripción | Ejemplo |
|---------|------------|---------|
| `ls` | Lista archivos y carpetas. | `$ ls` → `documento.txt imagen.jpg` |
| `ls -l` | Muestra detalles como permisos, propietario y fecha. | `$ ls -l` |
| `ls -a` | Incluye archivos ocultos en la lista. | `$ ls -a` → `.bashrc .profile` |
| `ls -lh` | Muestra tamaños en formato legible (KB, MB). | `$ ls -lh` → `10K documento.txt` |
| `ls -R` | Lista archivos y subdirectorios recursivamente. | `$ ls -R` |

---

## **📝 2. Manipulación de Archivos**  

| Comando | Descripción | Ejemplo |
|---------|------------|---------|
| `cat archivo.txt` | Muestra el contenido de un archivo. | `$ cat notas.txt` |
| `cat archivo1 archivo2` | Muestra ambos archivos juntos. | `$ cat notas1.txt notas2.txt` |
| `cp archivo.txt copia.txt` | Copia un archivo. | `$ cp notas.txt copia_notas.txt` |
| `cp -r carpeta destino/` | Copia una carpeta con todo su contenido. | `$ cp -r proyectos/ respaldo/` |
| `mv archivo.txt nueva_carpeta/` | Mueve un archivo a otra carpeta. | `$ mv notas.txt Documentos/` |
| `mv archivo.txt nuevo_nombre.txt` | Renombra un archivo. | `$ mv notas.txt notas_viejas.txt` |

---

## **🔍 3. Búsqueda y Filtros**  

| Comando | Descripción | Ejemplo |
|---------|------------|---------|
| `find /ruta -name "archivo.txt"` | Busca un archivo en una ruta específica. | `$ find /home/rafael -name "notas.txt"` |
| `find . -name "*.txt"` | Busca todos los archivos `.txt` en la ubicación actual. | `$ find . -name "*.txt"` |
| `grep "palabra" archivo.txt` | Busca una palabra dentro de un archivo. | `$ grep "error" log.txt` |
| `grep -r "palabra" /ruta` | Busca en todos los archivos de una ruta. | `$ grep -r "login" /var/logs` |

---

## **🔑 4. Permisos y Propietarios**  

| Comando | Descripción | Ejemplo |
|---------|------------|---------|
| `chmod 777 archivo.txt` | Permisos de lectura, escritura y ejecución para todos. | `$ chmod 777 script.sh` |
| `chmod +x script.sh` | Da permisos de ejecución a un archivo. | `$ chmod +x script.sh` |
| `chown usuario:grupo archivo.txt` | Cambia el propietario de un archivo. | `$ chown rafael:rafael notas.txt` |
| `chown -R usuario:grupo carpeta/` | Cambia el propietario de todos los archivos en una carpeta. | `$ chown -R rafael:rafael proyectos/` |

---

## **📊 5. Gestión de Procesos**  

| Comando | Descripción | Ejemplo |
|---------|------------|---------|
| `ps aux` | Muestra procesos en ejecución. | `$ ps aux` |
| `kill PID` | Finaliza un proceso por su ID. | `$ kill 1234` |
| `top` | Muestra procesos y consumo de recursos en tiempo real. | `$ top` |
| `htop` | Alternativa visual a `top` (requiere instalación). | `$ htop` |

---

## **💾 6. Gestión del Espacio en Disco**  

| Comando | Descripción | Ejemplo |
|---------|------------|---------|
| `df -h` | Muestra el espacio disponible en disco en formato legible. | `$ df -h` |
| `du -sh carpeta/` | Muestra el tamaño total de una carpeta. | `$ du -sh Descargas/` |

---

## **🛠️ 7. Compresión y Descompresión**  

| Comando | Descripción | Ejemplo |
|---------|------------|---------|
| `tar -cvf archivo.tar carpeta/` | Comprime una carpeta en `.tar`. | `$ tar -cvf backup.tar Documentos/` |
| `tar -xvf archivo.tar` | Extrae un archivo `.tar`. | `$ tar -xvf backup.tar` |
| `zip archivo.zip archivo.txt` | Comprime un archivo en `.zip`. | `$ zip notas.zip notas.txt` |
| `unzip archivo.zip` | Extrae un archivo `.zip`. | `$ unzip notas.zip` |

---

## **🌐 8. Conectividad y Descargas**  

| Comando | Descripción | Ejemplo |
|---------|------------|---------|
| `wget URL` | Descarga un archivo desde una URL. | `$ wget https://ejemplo.com/archivo.zip` |
| `curl -O URL` | Descarga un archivo con `curl`. | `$ curl -O https://ejemplo.com/archivo.zip` |

---

## **🔄 9. Alias y Personalización**  

| Comando | Descripción | Ejemplo |
|---------|------------|---------|
| `alias ll="ls -lah"` | Define un alias para un comando. | `$ alias ll="ls -lah"` |
| `unalias ll` | Elimina un alias. | `$ unalias ll` |
| `history` | Muestra el historial de comandos usados. | `$ history` |

---

## **🎯 10. Comandos Útiles Variados**  

| Comando | Descripción | Ejemplo |
|---------|------------|---------|
| `clear` | Limpia la pantalla de la terminal. | `$ clear` |
| `echo "Hola, mundo"` | Muestra un mensaje en la terminal. | `$ echo "Hola, mundo"` |
| `nano archivo.txt` | Edita un archivo con Nano. | `$ nano notas.txt` |
| `vim archivo.txt` | Edita un archivo con Vim. | `$ vim notas.txt` |
