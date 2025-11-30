Módulo-9-SO3-CLI Comandos utilizados en Laboratorio Módulo 9 - Sistemas Operativos III                                                                                                     
                                                                                                                                                                                          
Este repositorio contiene los comandos prácticos con los cuales se desarrollaron las prácticas de el noveno laboratorio de la asignatura Sistemas Operativos III, impartida por el profesor Adrian Alcantara.                                                                                                                                                                 
                                                                                                                                                                                          
En el mismo se desarrollaron los siguientes temas:                                                                                                                                         
                                                                                                                                                                                          
Practica 1: Instalacion de Webmin.                                                                                                                                                         
• Instalar Webmin.                                                                                                                                                                         
• Mostrar las opciones de administración que se pueden ejecutar vía Webmin:                                                                                                               
  • Administración de usuarios: Crear y eliminar una cuenta de usuario.                                                                                                                      • Gestión de servicios: Iniciar, detener y reiniciar servicios del sistema (ej. SSH).                                                                                                    
  • Configuración de red: Configurar una IP estática en interfaces de red.                                                                                           
  • Administración de software: Actualizar, instalar y eliminar alguna herramienta.                                                                                            
  • Gestión de archivos y directorios: Explorar, editar un archivo y eliminarlo.                                                                                                        
  • Monitorización del sistema: Supervisar el rendimiento del sistema (memoria, procesador, almacenamiento).                                                                                                                                                                                                                                                                          
Practica 2: Despliegue de una VM con Terraform en Digital Ocean.                                                                                                              
• Proceda a instalar Terraform en la VM Server:                                                                                                                              
  • https://developer.hashicorp.com/terraform/install                                                                                                               
• Desplegar una VM usando Terraform en Digital Ocean con las siguientes spec:                                                                                                   
  • image: ubuntu-22-04-x64                                                                                                                                                     
  • name: OS3vm                                                                                                                                                                    
  • region: nyc1                                                                                                                                                             
  • size: s-1vcpu-1gb                                                                                                                                                           
  • ssh_key: [llavePublicaDeTuServerAnsible]                                                                                                                                             
• Validar la creación de la VM ingresando vía SSH.                                                                                                                                      
• Validar también por el portal web de Digital Ocean que el despliegue se realizó de forma correcta.                                                                                      
                                                                                                                                                                                          
Practica 3: Instalación de Ansible.                                                                                                                    
• Instalar ansible en la VM-Server (que funcionará como ansible controller) junto a todas sus dependencias.                                                                
• Configurar ambos equipos clientes (la VM de Digital Ocean y la VM de Windows) para que sean compatibles con el ansible controller.                                             
• Crear un usuario llamado ansible con permisos de administrador (en el caso de Windows) y sudoers (en el caso de Linux).                                                            
• El usuario ansible puede iniciar sesión en ansible1 usando ssh, basándose en par de llaves ssh sin contraseña.                                                                     
• Crear un inventario de ansible (/etc/ansible/host) y crear un grupo llamado [win] para la pc de Windows y uno llamado [linux] para la VM de Linux.                                  
• Probar la conexión a ambos host utilizando el módulo ping.                                                                                                                          
                                                                                                                                                                                          
Practica 4: Comandos Ad-Hoc.
• Utilizando el módulo win_copy utilice un comando ad-hoc que copie un archivo txt ubicado en el escritorio de la máquina ansible2 a la carpeta de Documentos.  
• Utilizando el módulo reboot utilice un comando ad-hoc que reinicie la VM ansible1.  
                                                                                                                                                                                          
Practica 5: Playbooks.                                                                                                                                                                     
• Crear un playbook para instalar la aplicación notepad++ en la máquina ansible2 (Windows).                                                                                        
• Crear un playbook en la máquina ansible1 (Linux) para que instale NGINX e inicie el servicio.                                                                                          
                                                                                                                                                                                          
Este es el enlace a la lista de reproducción en YouTube correspondiente al Módulo 9: ↓                                                                                                    
https://youtube.com/playlist?list=PLn9wGcsdOtlerPJX8l0h4t9dRALFp4NeS&si=Cwm7L3gAlCaZ5b2E
