# ufw-rules
A script to execute the essential UFW rules.
ES 
# Configuración básica de UFW en Bash

Este script permite aplicar la configuración básica de seguridad del firewall UFW de forma automatizada mediante Bash.

## Objetivo 

El objetivo del script es establecer las políticas predeterminadas de UFW en modo bloqueo (deny) y permitir sólo los puertos necesarios para poder navegar y acceder de forma remota al sistema de forma segura.

## Uso

Para ejecutar el script se requieren permisos de root. Correr:

```
sudo bash ufw-config.sh
```

## Configuración

El script aplica la siguiente configuración de UFW:

- Habilita el firewall
- Establece políticas predeterminadas en deny para entrada y salida  
- Permite la salida a través de la interfaz eth0
- Permite los puertos 80, 443 y 22 entrantes desde cualquier IP

Este script está diseñado para configurar de forma básica UFW en sistemas Debian/Ubuntu y puede ser utilizado como punto de partida para implementar el firewall. Favor revisar y probar antes de usarlo en producción.

EN 
# Basic UFW configuration in Bash.

This script allows you to apply basic UFW firewall security configuration in an automated way using Bash.

## Objective. 

The goal of the script is to set the default UFW policies to block (deny) mode and allow only the necessary ports to securely browse and remotely access the system.

## Usage

To run the script root permissions are required. Run:

```
sudo bash ufw-config.sh
```

## Configuration

The script applies the following UFW configuration:

- Enables the firewall
- Sets default policies on deny for ingress and egress  
- Allow outbound through eth0 interface
- Allow incoming ports 80, 443 and 22 from any IP

This script is designed for basic UFW configuration on Debian/Ubuntu systems and can be used as a starting point for firewall implementation. Please review and test before using it in production.
