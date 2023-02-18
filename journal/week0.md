# Week 0 — Billing and Architecture

## Actividades a realizar
- [x] Visualizar los videos semanales
- [x] Crear usuario Admin
- [x] Generar las credenciales de AWS
- [x] Instalar AWS CLI
- [x] Crear Billing Alarm
- [x] Crear un Budget

## Creando el usuario Admin
<p>Para este caso utilizo mi nombre</p>
<image src="/images/user1.jpg" alt="Cuenta">
<p>Adicional a ello se agregan los perfiles necesarios</p>
<image src="/images/user2.jpg" alt="Perfiles asociados">

## Creando las credenciales de AWS

Previamente ingresamos a gitpod
<image src="/images/gitpod.jpg" alt="Pantalla de gitpod">

Para ello agregamos las siguientes claves en gitpod
gp env AWS_ACCOUNT_ID="1231245"
gp env AWS_ACCESS_KEY_ID="llavekey"
gp env AWS_SECRET_ACCESS_KEY="llavesecreta"
gp env AWS_DEFAULT_REGION="laregion" # e.g. us-east-1
gp env AWS_ACCOUNT_EMAIL="tu correo" 

Los comandos quedan registrados en el gitpod
<image src="/images/user-settings.jpg" alt="Comandos">
