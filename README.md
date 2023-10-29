# Ansible Configurar SSH

Este repositorio contiene un playbook de Ansible diseñado para facilitar la configuración de SSH en un servidor remoto. Con esta automatización, puedes copiar una clave pública SSH al servidor y reiniciar el servicio SSH para aplicar los cambios. El playbook solicita el nombre de usuario y la contraseña de sudo en el servidor remoto para completar la configuración.

## Uso

Siga estos pasos para utilizar este playbook:

1. Edite la etiqueta de hosts para incluir la dirección IP o el nombre de host del servidor remoto.
2. Asegúrese de que la clave pública SSH (generalmente id_rsa.pub) esté en su directorio ~/.ssh/.
3. Ejecute el playbook utilizando el siguiente comando, proporcionando la dirección IP o el nombre de host del servidor.
   
   ```bash
   ansible-playbook -i inventory.ini configurar_ssh.yaml

Siga las instrucciones para ingresar el nombre de usuario y la contraseña de sudo en el servidor remoto cuando se le solicite.
El playbook se encargará de copiar la clave pública SSH y reiniciar el servicio SSH en el servidor remoto, lo que permitirá la autenticación SSH con la clave.
