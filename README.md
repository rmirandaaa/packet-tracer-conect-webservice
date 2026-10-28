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
