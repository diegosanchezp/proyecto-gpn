# Apertura de cuentas bancarias

Proyecto GPN 2-2021

## Instalación

Instalación en linux
1. Descargar el archivo `AperturaCuentaBancaria_20220212_1053.bos`
2. Abrir Bonita Studio
3. Abrir archivo `AperturaCuentaBancaria_20220212_1053.bos` en Bonita Studio
   ```
   File > Import > Bos archive
   ```
   - Seleccionar archivo `AperturaCuentaBancaria_20220212_1053.bos`
   - Asegurate de que tenga el nombre `AperturaCuentaBancaria`
   - Clic details
   - Clic extensions
   - Clic import 
   - Con eso se deberia de importar el archivo

4. Ir a la carpeta de donde se instaló Bonita Studio
```bash
# Especifica la carpeta de instalación de Bonita
# en esta variable, el valor es un ejemplo
BONITA_DIR=$HOME/BonitaStudioCommunity-2021.2-u0

cd $BONITA_DIR/workspace/AperturaCuentaBancaria
rm -r .project diagrams/ environements/ organizations/ process_configurations/ target/ pom.xml
git init
git remote add origin git@github.com:diegosanchezp/proyecto-gpn.git
git pull origin master
```

Verificar que aparezcan los diagramas en Proccess diagramas
![verificar-aparezcan-diagramas.png](verificar-aparezcan-diagramas.png)
