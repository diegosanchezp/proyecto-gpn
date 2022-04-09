# Dependencias de sistema
Dependencias de sistema que hay que instalar para los conectores de Bonita

- Un Servidor SMTP escuchando en `localhost`, puerto `2525`

Yo estoy utilizando [smtp4dev](https://github.com/rnwood/smtp4dev), lo instale via docker, siguiendo estas [instrucciones](https://github.com/rnwood/smtp4dev/wiki/Installation#how-to-run-smtp4dev-in-docker)
``
# Pasos para ejecutar el proceso de apertura de cuenta bancaria
1. Instalar las dependencias de sistema
2. Abrir el diagrama **Apertura de Cuenta (1.0)** con Bonita Studio

Estos pasos son en la GUI de Bonita Studio, se ejecutan en el taskbar ubicado en la parte superior
3. Desplegar el modelo de base datos
	1. Development > Business Data Model > Clean Deploy
4. Desplegar organization
	1. Organization > Deploy
	2. Seleccionar Banco XYZ
	3. Clic deploy
	
Cuando se ejecuta el proceso, se pueden loguear dos usuarios, estos son las credenciales

Usuario tipo que realiza solicitud
	username: cliente
	password: bpm
	
Usuario que revisa las solicitudes bancarias (agente bancario)
	username: inspector
	password: bpm