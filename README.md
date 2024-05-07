# Hacking de Redes Wi-Fi

Necesitaras los siguientes programa instalados:


https://www.vmware.com/products/workstation-player/workstation-player-evaluation.html.html.html


Descargar Kali Linux:
En nustro caso Utilizamos VMware


https://www.kali.org/get-kali/#kali-virtual-machines


Informacion basica:
<p>Kali linux es una distribución basada en debian, cuenta con diversas herramientas enunciare algunos usos de las mismas.</p>

<li>Recopilacion de Informacion</li>

<li>Analisis de Vulnerabilidad</li>

<li>Ataques Inalambricos</li>

<li>Ataques a aplicaciones Web</li>

<li>Analisis forense digital</li>


<h4>Ejecutamos adentro de la consola: ifconfig</h4>

<p>Podemos visualizar la interfaz de red *eth0* significa que es una tarjeta red tipo *Ethernet* es decir alambrica, Kali en la maquina VMware independientemente que este nuestro pc conectado a wifi lo reconoce como eth0 por eso necesitaremos una tarjeta de red externa.</p>

Para estos  en caso de no contar con una antena la informacion aca se esta realizando con una AC600 TP-LINK:


![imagen](https://github.com/SantiagoBaquero/Hacking-de-Redes-Wi-Fi/assets/102531445/024293a1-0f5c-4f15-b3d5-ecba4428a376)


Una vez esta sea conecta al equipo nos saldra una ventana donde seleccionamos que nuestro adaptador de red Wi-Fi externo sea utilizado en la maquina virtual:

![imagen](https://github.com/SantiagoBaquero/Hacking-de-Redes-Wi-Fi/assets/102531445/658e32cf-6904-4579-8a53-d1956c7e15ed)

Una vez realizado esto para comprobar que este en funcionamiento buscaremos una red como se muestra en la imagen donde podemos visualizar diferentes redes alrededor de mi ubicacion:

![imagen](https://github.com/SantiagoBaquero/Hacking-de-Redes-Wi-Fi/assets/102531445/9ccba1f2-f0e3-49bd-b333-b44ed82284eb)

Una vez ejecutemos nuevamente el comando en la consola *ifconfig* podremos apreciar que aparece el Wlan0

![imagen](https://github.com/SantiagoBaquero/Hacking-de-Redes-Wi-Fi/assets/102531445/b1039cdf-3ffc-4379-ace2-5be9c00853d7)



# Direccion Mac
Direccion Utilizada en la capa 2 del modelo ISO OSI.
Identificador de 48 bits se encuentra en 6 bloques de dos caracteres hexadecimales, tambien es conocida como la direccion fisica es unico por cada tarjeta.

![imagen](https://github.com/SantiagoBaquero/Hacking-de-Redes-Wi-Fi/assets/102531445/a0311e5a-7f63-4ecf-91c2-a6f09b84aaed)

<sub>Imagen extraida de: [Computerhoy.com 6/05/2024] (https://computerhoy.com/reportajes/tecnologia/direccion-mac-ordenador-movil-sirve-317181) </sub>



# Spoofing
<h3>El atacante puede cambiar su direccion MAC y hacerse pasar por otro dispositivo.</h3> 
<p>Lo que ocasiona que cuando el dispositivo reciba el paquete piense que este viene del access point de confianza.</p> 
  
Para cambiar la direccion MAC lo podemos realizar de la siguiente forma ejecutar el comando en consola *ifconfig* este nos mostrata la direccion MAC de nuestra tarjeta.
En la imagen se muestrea donde podemos ubicar la direccion MAC 
![imagen](https://github.com/SantiagoBaquero/Hacking-de-Redes-Wi-Fi/assets/102531445/f92bc70b-4c0a-414b-8629-201aee67ae7e)


<p>Siguiente comando: <strong>ifconfig wlan0 down</strong>  <br> Con este comando desactivamos la interfaz de red wlna0 (puede solicitar super usuario "sudo su") <br> Siguiente comando: <strong>ifconfig wlan0 hw ether</strong>(dirección mac) -> <strong>ifconfig wlan0 hw ether 00:11:22:33:44:55</strong>  <br> Siguiente comando: <strong>ifconfig wlan0 up</strong> (Habilitamos la interfaz)   </p>

![imagen](https://github.com/SantiagoBaquero/Hacking-de-Redes-Wi-Fi/assets/102531445/78dbe0f9-b8db-4b63-9711-3499e416c9d6)


<p>En caso de que el cambio no se mantenga utilice el comando: <strong>servie NetworkManager stop</strong>  posterior a esto los comandos previamente mencionados y para finalizar <strong>servie NetworkManager start</strong> </p>

# Sniffing

  




