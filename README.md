# ords-oracle-install

## Pasos para instalar ORDS-ORACLE

#### 1. Debemos copiar dos archivos a los servidores donde queremos instalar los ords
> Como recomendacion ambos archivos podemos copiar en el path /tmp ya que alli se alojan los archivos temporales.

[ ]  jdk.zip

[ ] ords.war

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
#### 3. En el path /tmp ejecutamos el siguiente comando
> De esta manera abrimos el archivo ords.war con el jdk que copiamos
```powershell
/usr/java/jdk11.0.12/bin/java -jar ords.war install
```
#### Nos aparecera el siguiente mensaje

>Enter number for [1] Basic  [2] TNS  [3] Custom URL [1]:1

1. Seleccionamos 1 y damos enter

> Enter the name of the database server [localhost]:se ingresa el nombre del servidor donde esta la base de datos ej [pl-veyco-dboc1]

2. Damos enter

> Enter the database listen port [1521]: enter si es que el puerto esta correcto

3. Damos enter

> Enter the database service name: [nos provee base de datos] EJ. timmy.PROD
