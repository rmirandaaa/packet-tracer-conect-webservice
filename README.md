# Packet Tracer: Conectarse a un Servidor Web

Práctica de laboratorio orientada a la verificación de conectividad y análisis del flujo de paquetes IP utilizando Cisco Packet Tracer.

---

## Objetivos
* Observar y comprender cómo se envían los paquetes a través de la red utilizando direcciones IP.
* Comprobar la comunicación end-to-end entre un host de origen y un servidor web mediante comandos de red y herramientas de cliente.

---

## Instrucciones y Desarrollo de la Práctica

### Parte 1: Verifique la conectividad con el servidor Web
1. **Abrir la terminal del host:** Seleccione `PC0`, vaya a la pestaña **Desktop** y abra **Command Prompt** (Línea de comandos).
2. **Prueba de conectividad (Ping):** Ejecute el comando de eco hacia la dirección IP asignada al servidor web (`172.33.100.50`):
   ```cmd
   ping 172.33.100.50

---

## Resultado obtenido en la simulación:
Pinging 172.33.100.50 with 32 bytes of data:

Reply from 172.33.100.50: bytes=32 time=0ms TTL=127
Reply from 172.33.100.50: bytes=32 time=0ms TTL=127
Reply from 172.33.100.50: bytes=32 time=0ms TTL=127
Reply from 172.33.100.50: bytes=32 time=0ms TTL=127

Ping statistics for 172.33.100.50:
Packets: Sent = 4, Received = 3, Lost = 1 (25% loss),
Approximate round trip times in milli-seconds:
Minimum = 0ms, Maximum = 0ms, Average = 0ms

## Nota técnica
* Nota técnica: Una respuesta exitosa verifica la conectividad lógica entre el cliente y el servidor.
* Es común que el primer paquete sufra un Request timed out (pérdida del 25% en este caso) mientras los dispositivos convergen y se resuelven las direcciones físicas mediante el protocolo ARP.

### Parte 2: Conéctese con el servidor Web a través del cliente Web
* Dentro de la pestaña Desktop de PC0, abra la aplicación Web Browser (Navegador web).
* Ingrese la dirección IP 172.33.100.50 en la barra de URL y haga clic en Go. El cliente web establecerá la conexión HTTP con el servidor utilizando la dirección IP.

### Pregunta de análisis:
¿Qué mensajes se ven después de que la página web se terminó de cargar?

Al cargar la página correctamente, se visualiza el siguiente mensaje institucional del servidor:

**"Welcome to the Learn IP Web Site"
"You were able to reach this website because you had the IP address of the web server. The connecting PC also had a web client running on the device."**
