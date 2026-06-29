# TP3 Cloud - Sistemas Operativos

Repositorio para realizar el Trabajo Práctico 3 de Sistemas Operativos usando GitHub Codespaces como infraestructura cloud.

## Entorno cloud seleccionado

Se utiliza GitHub Codespaces con una configuración de Dev Container basada en Fedora Linux.

La configuración se encuentra en:

```text
.devcontainer/devcontainer.json
```

## Comandos para las capturas del TP

### 1. Verificar sistema operativo

```bash
cat /etc/os-release
uname -a
hostnamectl
```

### 2. Ver recursos asignados

```bash
lscpu
free -h
df -h
```

### 3. Verificar conexión a internet

```bash
curl -I https://www.google.com
```

### 4. Crear archivo de prueba

```bash
mkdir tp3_cloud
cd tp3_cloud
echo "Archivo de prueba creado en infraestructura cloud" > prueba_cloud.txt
cat prueba_cloud.txt
```

### 5. Verificar persistencia

Cerrar el Codespace, volver a abrirlo y ejecutar:

```bash
cat tp3_cloud/prueba_cloud.txt
```

### 6. Instalar aplicación

```bash
sudo dnf update -y
sudo dnf install htop -y
htop --version
```

### 7. Seguridad y usuario

```bash
whoami
id
ls -la
```

## Objetivo

Demostrar el uso de una infraestructura cloud para ejecutar un entorno Linux, consultar recursos del sistema, acceder a internet, crear archivos persistentes e instalar aplicaciones.
