# ords-oracle-install

## Pasos para instalar ORDS-ORACLE

#### 1. Debemos copiar dos archivos a los servidores donde queremos instalar los ords

> jdk.zip

> ords.war

#### 1. Descomprimir el archivo jdk11.0.12.zip
```powershell
unzip jdk.zip
```
#### 2. Creamos el directorio java en /usr
> Damos permisos de ejecucion al directorio
```powershell
chmod -R 755
```
```powershell
mkdir /usr/java
```
#### 2. Copiamos el archivo descomprimido en el path /usr/java
```powershell
cp -av [jdk_descomprimido] /usr/java
```
