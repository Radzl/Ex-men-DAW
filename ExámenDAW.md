# **Exámen DAW**

---

## **Índice**

1. **Tipo test**

2. **SSH + Command line**

3. **Virtual Host**

--- 
### **Tipo test**

>El apartado de tipo test ha sido contestado mediante información de los apuntes y de webs confiables con información sobre Markdown y 
comandos de Ubuntu como [Hostinger](https://www.hostinger.es/tutoriales/linux-comandos) y [Guía Ubuntu](https://www.guia-ubuntu.com/index.php/Comandos).

### **SSH + Command line**

>**Título de la actividad:**
Deberás ir al escritorio y crear un archivo de texto que contenga como nombre de archivo, 
tu nombre propio y apellido sin espacios y con extensión txt (por ejemplo ArnoldSchwarzenegger.txt) escribe en su interior el resultado de whoami.
Después, mediante otro comando, concatena al final del archivo el nombre del comando necesario para saber quién está conectado a la máquina mediante ssh.

>A continuación detallaré los comandos ejecutados, con sus respectivos comentarios aclarativos para llevar a cabo la actividad.

1. **sudo apt install openssh-server** 
2. **ssh usuario@192.168.0.185** 
3. **password usuario : DAMWDAWM** (Pedirá la contraseña de usuario, la cual es: DAMWDAWM)
4. **cd Escritorio** (Nos permitirá situarnos en el escritorio)
5. **touch RaduAndreiO.txt** (Nos permitirá crear el archivo RaduAndreiO.txt)
6. **nano RaduAndreiO.txt** (Nos permitirá añadir la información de la actividad, es decir, el resultado de whoami -> usuario, y además el comando who -> permite ver quien hay conectado mediante ssh)
7. **cat RaduAndreiO.txt** (Verificar)

### **Virtual Host**

>**Título de la actividad:**
Documenta todos los pasos realizados en un archivo MarkDown. Crea en tu máquina un virtualhost donde escribiendo “daw.ejercicio3.com” nos envíe a una web local ubicada en /var/www/miWeb, y que el correo de administrador sea el tuyo. No cierres la máquina al acabar el examen para poder comprobar su funcionamiento.

>A continuación detallaré los comandos ejecutados y comentarios aclarativos para llevar a cabo la actividad.

1. **sudo apt update** (Actualizaciones)
2. **sudo apt install apache2** (Instalar apache)
3. **sudo mkdir -p /var/www/radu.com/Examen** (Crear carpeta Examen)
4. **sudo chown -R $USER:$USER /var/www/radu.com/Examen** (Conceder permisos)
5. **sudo chmod -R 755 /var/www** (Garantizar el acceso a lectura)
6. **nano /var/www/radu.com/Examen/index.html** (Abrir index.html)
7. **nano /var/www/radu.com/Examen/index.html** (Modificar info)
8. **sudo nano /etc/apache2/sites-available/radu.com.conf** (Editor privilegios)
9. **Ctrl+/**  (Reemplazar el correo por defecto por radudaw1@gmail.com)







