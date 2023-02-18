# Week 0 — Billing and Architecture

## Actividades a realizar
- [x] Visualizar los videos semanales
- [x] Crear usuario Admin
- [x] Generar las credenciales de AWS
- [x] Instalar AWS CLI
- [x] Crear Billing Alarm
- [x] Crear un Budget
- [x] Diagrama Lógico
- [x] Diseño Conceptual

## Creando el usuario Admin
<p>Para este caso utilizo mi nombre</p>
<image src="/images/user1.jpg" alt="Cuenta">
<p>Adicional a ello se agregan los perfiles necesarios</p>
<image src="/images/user2.jpg" alt="Perfiles asociados">

## Creando las credenciales de AWS

<p>Previamente ingresamos a gitpod</p>
<image src="/images/gitpod.jpg" alt="Pantalla de gitpod">

<p>Para ello agregamos las siguientes claves en gitpod</p>

- [x] gp env AWS_ACCOUNT_ID="1231245"
- [x] gp env AWS_ACCESS_KEY_ID="keyid"
- [x] gp env AWS_SECRET_ACCESS_KEY="llavesecreta"
- [x] gp env AWS_DEFAULT_REGION="laregion" # ex. us-east-1
- [x] gp env AWS_ACCOUNT_EMAIL="tu correo" 

<p>Las variables de entorno quedan registradas en el gitpod</p>
<image src="/images/user-settings.jpg" alt="Comandos">

## Instalar AWS CLI

<p>Para instalar AWS CLI se usa el siguiente script dentro de .gitpod.yml</p>

```yml
tasks:
  - name: aws-cli
    env:
      AWS_CLI_AUTO_PROMPT: on-partial
    init: |
      cd /workspace
      curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
      unzip awscliv2.zip
      sudo ./aws/install
      cd $THEIA_WORKSPACE_ROOT
```

## Crear Billing Alarm
<p>Creamos una Billing Alarm en la consola de AWS</p>
<image src="/images/billing.jpg" alt="Billing">

## Crear Budget
<p>Creamos un Budget en la consola de AWS</p>
<image src="/images/budget.jpg" alt="Budget">

## Diagrama Lógico
<p>El enlace se encuentra en la ruta:</p>
https://lucid.app/lucidchart/29e41842-6705-455f-a34f-1ab2ab5e8d06/edit?viewport_loc=-476%2C-233%2C2303%2C1146%2C0_0&invitationId=inv_e99b5908-f1af-41a5-a4b9-367f627f819b
<image src="/images/logical.jpeg" alt="Diagrama logico">

## Diseño Conceptual
<p>El enlace se encuentra en la ruta:</p>

<image src="/images/conceptual.jpeg" alt="Diseño Conceptual">