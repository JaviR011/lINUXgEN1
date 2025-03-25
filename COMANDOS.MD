

### 1. `ls` – Lista archivos y directorios
```bash
ls               # Lista archivos en el directorio actual
ls -l            # Lista detalladamente (permisos, propietario, etc.)
ls -a            # Muestra archivos ocultos
```

### 2. `cd` – Cambia de directorio
```bash
cd Documentos/   # Entra al directorio Documentos
cd ..            # Sube un nivel
cd ~             # Va al directorio personal del usuario
```

### 3. `pwd` – Muestra el directorio actual
```bash
pwd              # Muestra la ruta actual
cd /etc && pwd   # Navega y muestra ruta
cd ~ && pwd      # Muestra ruta al home
```

### 4. `mkdir` – Crea directorios
```bash
mkdir nueva_carpeta
mkdir -p carpeta1/carpeta2  # Crea subdirectorios recursivamente
mkdir {a,b,c}               # Crea múltiples carpetas a la vez
```

### 5. `rmdir` – Elimina directorios vacíos
```bash
rmdir carpeta_vacia
rmdir -p carpeta1/carpeta2  # Elimina si ambas están vacías
rmdir {a,b,c}               # Elimina múltiples carpetas vacías
```

### 6. `rm` – Elimina archivos o carpetas
```bash
rm archivo.txt
rm -r carpeta               # Elimina carpeta y contenido
rm -f archivo.txt           # Elimina sin pedir confirmación
```

### 7. `cp` – Copia archivos o carpetas
```bash
cp archivo.txt copia.txt
cp -r carpeta1 carpeta2     # Copia recursivamente una carpeta
cp *.txt backup/            # Copia todos los .txt al folder backup
```

### 8. `mv` – Mueve o renombra archivos
```bash
mv archivo.txt carpeta/         # Mueve archivo
mv viejo.txt nuevo.txt          # Renombra archivo
mv *.jpg imagenes/              # Mueve todos los .jpg
```

### 9. `touch` – Crea archivos vacíos
```bash
touch nuevo.txt
touch archivo{1..3}.txt         # Crea archivo1.txt a archivo3.txt
touch -c archivo.txt            # No crea si no existe
```

### 10. `file` – Muestra tipo de archivo
```bash
file imagen.jpg
file script.sh
file binario                 # Verifica tipo de archivo
```

### 11. `find` – Busca archivos/directorios
```bash
find . -name "*.txt"
find /etc -type d -name "ssh*"
find . -size +1M              # Archivos mayores a 1MB
```

### 12. `locate` – Localiza archivos rápidamente
```bash
locate bashrc
locate *.jpg | head
locate -i documento           # Búsqueda sin distinguir mayúsculas
```

### 13. `tar` – Archiva y descomprime archivos .tar
```bash
tar -cvf archivo.tar carpeta/
tar -xvf archivo.tar
tar -czvf archivo.tar.gz carpeta/
```

### 14. `zip` / `unzip` – Comprime y descomprime archivos
```bash
zip archivos.zip *.txt
unzip archivos.zip
zip -r carpeta.zip carpeta/
```

### 15. `cat` – Muestra contenido de archivos
```bash
cat archivo.txt
cat archivo1 archivo2 > fusion.txt
cat -n archivo.txt        # Muestra con número de línea
```

### 16. `head` / `tail` – Muestra primeras o últimas líneas
```bash
head archivo.txt
tail archivo.txt
tail -f log.txt           # Muestra en tiempo real
```

### 17. `grep` – Busca patrones en texto
```bash
grep "error" log.txt
grep -i "usuario" archivo.txt
grep -r "clave" ./         # Busca recursivamente
```

### 18. `awk` – Procesa texto en columnas
```bash
awk '{print $1}' archivo.txt
awk -F: '{print $1, $3}' /etc/passwd
awk '/root/ {print $0}' /etc/passwd
```

### 19. `sed` – Edita texto en archivos
```bash
sed 's/viejo/nuevo/' archivo.txt
sed -n 2,4p archivo.txt     # Muestra líneas 2 a 4
sed '/^$/d' archivo.txt     # Elimina líneas vacías
```

### 20. `set` – Muestra variables del entorno
```bash
set
set | grep PATH
set nombre=valor
```

### 21. `chmod` – Cambia permisos de archivo
```bash
chmod +x script.sh
chmod 755 archivo
chmod -R 644 carpeta/*
```

### 22. `chown` – Cambia propietario de archivos
```bash
chown usuario archivo
chown usuario:grupo archivo
chown -R usuario carpeta/
```

### 23. `sudo` – Ejecuta como administrador
```bash
sudo apt update
sudo rm archivo_sistema
sudo systemctl restart nginx
```

### 24. `df` – Muestra uso de disco
```bash
df
df -h                # Formato legible
df /home             # Espacio en partición específica
```

### 25. `du` – Muestra tamaño de carpetas
```bash
du -sh carpeta/
du -ah | sort -h
du -csh *            # Total de tamaños en carpeta
```

### 26. `uname` – Muestra información del sistema
```bash
uname
uname -r            # Versión del kernel
uname -a            # Detalles completos
```

### 27. `date` – Muestra o configura fecha/hora
```bash
date
date "+%Y-%m-%d %H:%M:%S"
date -s "25 MAR 2025 14:00:00"
```

### 28. `who` – Muestra usuarios conectados
```bash
who
whoami
who -b              # Último reinicio
```

### 29. `id` – Muestra UID y grupos
```bash
id
id usuario
id -g               # Solo el grupo
```

### 30. `echo` – Muestra texto o variables
```bash
echo "Hola mundo"
echo $HOME
echo "User: $USER, Dir: $PWD"
```

### 31. `source` – Ejecuta script en shell actual
```bash
source script.sh
source ~/.bashrc
. config.sh        # Forma corta de `source`
```

### 32. `type` – Verifica tipo de comando
```bash
type ls
type -a echo
type grep
```

### 33. `man` – Manual de comandos
```bash
man ls
man grep
man -k copy         # Buscar por palabra clave
```

### 34. `help` – Ayuda para comandos internos
```bash
help cd
help echo
help if             # Ayuda para estructuras shell
```

### 35. `export` – Exporta variables al entorno
```bash
export MI_VAR=123
echo $MI_VAR
export PATH=$PATH:/mi/ruta
```


