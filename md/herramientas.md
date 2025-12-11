# Herramientas de Redes

Estas son las herramientas más utilizadas para diagnosticar y analizar redes.

---

## Ping
Comprueba si un dispositivo responde.

```yaml
ping 8.8.8.8
```

---

## Tracert / Traceroute
Muestra el recorrido de un paquete hasta un destino.

```yaml
traceroute google.com # Linux
tracert google.com # Windows
```

---

## Ipconfig / Ifconfig / IP
Muestra la configuración de red.

```yaml
Windows:
ipconfig

Linux:
ifconfig
ip a
```

---

## Nslookup
Consulta registros DNS.

```yaml
nslookup google.com
```

---

## Netstat
Muestra conexiones activas.

```yaml
netstat -an
```

---

## Nmap
Escaneo de puertos y redes.

```yaml
nmap 192.168.1.0/24
```

!!! tip "Consejo"
    Estas herramientas permiten detectar problemas y analizar el estado de cualquier red.