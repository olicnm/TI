Konnektor und Firewalls: Offene Ports für eine Anbindung an die TI


Wird ein lokales Leistungserbringernetz durch eine eigene Firewall gesichert, hinter der der Konnektor zur TI-Anbindung betrieben werden soll (Parallelschaltung), sollten die folgenden ausgehenden Ports in der Firewall für Routen in Richtung TI geöffnet werden:

    Vom Konnektor ausgehend in Richtung Internet (outbound)

DNS (UDP/TCP 53) z.B. Verbindung mit VPN-Zugangsdienst
HTTP (TCP 80) z.B. Aktualisierung der CRL
HTTPS-alt (TCP 8443) z.B. Registrierung des Konnektors am Registrierungsserver
isakmp (UDP 500) VPN-Tunnel
isakmp-nat-t (UDP 4500) VPN-Tunnel
ICMP-Ping (Typ 8 Code 0)


    Innerhalb der Praxis (eingehend und ausgehend)



    Zwischen dem Konnektor und der Praxisverwaltungssoftware (PVS):

HTTP/S (TCP 80/443)
SOAP (TCP 8200/8400)
CETP (PVS Spezifisch(?))
LDAP/S (TCP 389/636)


    Zwischen dem Konnektor und dem Kartenterminal:

SICCT (UDP 4742)
