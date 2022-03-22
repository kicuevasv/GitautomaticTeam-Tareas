
Tarea 3 - Comandos básicos de gcloud

1.- Listar Compute Engine

2.- Listar IP’s en uso, existentes o reservadas

3.- Listar buckets disponibles

4.- Listar Service Accounts existentes en un proyecto
## ¿Qué es una cuenta de servicio?
Una cuenta de servicio es un tipo especial de cuenta que usa una carga de trabajo de aplicación o procesamiento, en lugar de una persona. Las cuentas de servicio se administran mediante la administración de identidades y accesos (IAM).

## Tipos de cuentas de servicio:
##### 1. Cuentas de servicio administradas por el usuario
##### 2. Cuentas de servicio administradas por Google

### 1. Cuentas de servicio administradas por el usuario
     Las cuentas de servicio administradas por el usuario incluyen cuentas de servicio nuevas que creas explícitamente y la cuenta de servicio predeterminada de            Compute Engine.

#### Cuentas de servicio nuevas
     Usa IAM para crear y administrar tus propias cuentas de servicio. Después de crear una cuenta, otórgale roles de IAM y configura instancias para que se ejecuten        como cuenta de servicio. Las aplicaciones que se ejecutan en instancias con la cuenta de servicio adjunta pueden usar las credenciales de la cuenta para realizar      solicitudes a otras API de Google.

### 2. Cuentas de servicio administradas por Google
    Estas cuentas de servicio (a veces conocidas como agentes de servicio) las crea y administra Google, y se asignan a tu proyecto automáticamente. Estas cuentas         representan diferentes servicios de Google y cada cuenta tiene cierto nivel de acceso a tu proyecto de Google Cloud

#### Agente de servicios de las API de Google
     Además de la cuenta de servicio predeterminada, todos los proyectos habilitados con Compute Engine tienen un agente de servicio de las API de Google, que se puede      identificar mediante el correo electrónico:
     PROJECT_NUMBER@cloudservices.gserviceaccount.com
     Esta cuenta de servicio está diseñada específicamente para ejecutar procesos internos de Google en tu nombre.
     Esta cuenta de servicio solo se borra cuando se borra el proyecto

#### Agente de servicio de Compute Engine
     Todos los proyectos que habilitaron la API de Compute Engine tienen un agente de servicio de Compute Engine, que tiene el siguiente correo electrónico:
     service-PROJECT_NUMBER@compute-system.iam.gserviceaccount.com
     Esta cuenta de servicio está diseñada específicamente para que Compute Engine realice las tareas de servicio en tu proyecto. Se basa en la Política de IAM 

     


Al final, añadir las URLs de las cuales obtuvieron la información.
