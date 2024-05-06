# Hacking de Redes Wi-Fi

Necesitaras los siguientes programa instalados:


https://www.vmware.com/products/workstation-player/workstation-player-evaluation.html.html.html


Descargar Kali Linux:
En nustro caso Utilizamos VMware


https://www.kali.org/get-kali/#kali-virtual-machines


Informacion basica:
Kali linux es una distribución basada en debian, cuenta con diversas herramientas enunciare algunos usos de las mismas.

-Recopilacion de Informacion

-Analisis de Vulnerabilidad

-Ataques Inalambricos

-Ataques a aplicaciones Web

-Analisis forense digital


Ejecutamos adentro de la consola: ifconfig

Podemos visualizar la interfaz de red *eth0* significa que es una tarjeta red tipo *Ethernet* es decir alambrica, Kali en la maquina VMware independientemente que este nuestro pc conectado a wifi lo reconoce como eth0 por eso necesitaremos una tarjeta de red externa.

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




