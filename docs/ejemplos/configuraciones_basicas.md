# Configuraciones Básicas

En esta sección veremos ejemplos reales de configuraciones simples tanto en Windows como en Linux.

---

# Configurar una IP estática en Windows

1. Abrir **Panel de control**.
2. Ir a *Centro de redes*.
3. Seleccionar la conexión (Ethernet o Wi-Fi).
4. Pulsar en **Propiedades**.
5. Seleccionar **Protocolo IPv4**.
6. Introducir:
    IP: 192.168.1.50
    Máscara: 255.255.255.0
    Puerta de enlace: 192.168.1.1
    DNS: 8.8.8.8

---

# Configurar una IP estática en Linux (Ubuntu)

Editar el archivo: sudo nano /etc/netplan/01-network-manager-all.yaml

Ejemplo:

```yaml
network:
  ethernets:
    enp0s3:
      addresses: [192.168.1.40/24]
      gateway4: 192.168.1.1
      nameservers:
        addresses: [8.8.8.8]
  version: 2

Aplicar cambios: sudo netplan apply
---

## **📌 herramientas.md (REHECHO)**
```markdown
# Herramientas de Redes

Estas son las herramientas más utilizadas para diagnosticar y analizar redes.

---

## ping
Comprueba si un dispositivo responde.

ping 8.8.8.8

yaml
Copiar código

---

## tracert / traceroute
Muestra el recorrido de un paquete hasta un destino.

traceroute google.com # Linux
tracert google.com # Windows

yaml
Copiar código

---

## ipconfig / ifconfig / ip
Muestra la configuración de red.

Windows:
ipconfig

makefile
Copiar código

Linux:
ifconfig
ip a

yaml
Copiar código

---

## nslookup
Consulta registros DNS.

nslookup google.com

yaml
Copiar código

---

## netstat
Muestra conexiones activas.

netstat -an

yaml
Copiar código

---

## nmap
Escaneo de puertos y redes.

nmap 192.168.1.0/24

markdown
Copiar código

> Estas herramientas permiten detectar problemas y analizar el estado de cualquier red.