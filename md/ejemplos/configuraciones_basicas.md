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
```

Aplicar cambios: sudo netplan apply