# gestion-paquetes
Gestión de paquetes

* Modifica la configuración de red de DHCP a estática
Para ello vamos a modificar el fichero /etc/sysconfig/network-scripts/ifcfg-enp1s0 en mi caso ya que la interfaz de mi red se llama enp1s0.
![conf_red](/images/conf_red.png)
Y vamos a añadir el siguiente bloque.
<pre>BOOTPROTO=static
DEVICE=eth0
ONBOOT=yes
TYPE=Ethernet
USERCTL=no
IPADDR=X.X.X.X
NETMASK=X.X.X.X
GATEWAY=X.X.X.X
DNS1=X.X.X.X
DNS2=X.X.X.X
DNSX=X.X.X.X</pre>
* Actualiza el sistema a las versiones más recientes de los paquetes instalados     
* Instala los repositorios adicionales EPEL y CentOSPlus     
* Instala el paquete que proporciona el programa dig, explicando los pasos que has dado para encontrarlo     
* Explica qué comando utilizarías para ver la información del paquete kernel instalado     
* Instala el repositorio adicional "elrepo" e instala el último núcleo disponible del mismo (5.9.X)     
* Busca las versiones disponibles para instalar del núcleo linux e instala la más nueva     
* Muestra el contenido del paquete del último núcleo instalado
