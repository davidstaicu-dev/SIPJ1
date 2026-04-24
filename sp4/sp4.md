---
layout: default
title: "A1. Sprint 4: Monitorització, connexió remota i llicenciament"
---

# Monitorització

## Monitor del sistema
Tenim el monitor del sistema d'Ubuntu per a monitorar recursos de forma general:

<img width="696" height="499" alt="image" src="https://github.com/user-attachments/assets/46fbc53c-4938-40d9-a33f-9b9d6bf87df5" />
<img width="696" height="499" alt="image" src="https://github.com/user-attachments/assets/83b6bea6-4416-4860-9f96-7ba9ff3f610d" />
<img width="696" height="499" alt="image" src="https://github.com/user-attachments/assets/b96840c6-9c91-4032-a50e-71873263a9e3" />

## Syslog

Aquí es guarden diversos logs (registres) com autentificació d'usuaris, inici del sistema, kernel, el gran journal, etc. Coses que instal·lem, els seus logs es desen aquí.
Diversos arxius comprinits aquí s'anomenen "Notació de logs", ja que són tants que per espai i organització es desen així.

## logrotate.conf

Aquí es pot configurar la rotació dels logs, cada quan volem registrar x events. En el seu directori hi ha arxius de configuració per cada servei.

## rsyslog

50-default.conf
<img width="810" height="578" alt="image" src="https://github.com/user-attachments/assets/1b287ed2-aa7f-4469-b337-84e86e750286" />


## logger
<img width="816" height="159" alt="image" src="https://github.com/user-attachments/assets/20a494ab-39a4-43eb-9c4d-4cfc99f5dc4b" />

Cambiem * del mail a "=crit":
<img width="862" height="578" alt="image" src="https://github.com/user-attachments/assets/d0407bcd-d2aa-4532-bba7-16a59bb9bc4c" />

Cal fer un "sudo systemctl restart rsyslog.service".

I ara no s'ha desat el log amb .alert, sols el .crit:
<img width="866" height="252" alt="image" src="https://github.com/user-attachments/assets/f6b37dac-93c1-4e7c-8a82-4d2bfc04f7de" />

## david.log

<img width="617" height="130" alt="image" src="https://github.com/user-attachments/assets/0ae64bd3-5bd5-4be5-8588-947dc02201e8" />

<img width="828" height="247" alt="image" src="https://github.com/user-attachments/assets/71cbb654-7441-4cec-8a1e-a6482a545703" />


# SSH

El primer es instalar aquests paquests en ambdues màquines, un permet connectar-se i l'altres que es connectin.

<img width="703" height="117" alt="imatge" src="https://github.com/user-attachments/assets/c3125d41-8b43-49d3-b173-650c837d3e01" />

A partir d'això es pot executar la comanda "ssh *usuari@IP*" per connectar-se remotament a altres màquines de la mateixa xarxa.

<img width="738" height="477" alt="imatge" src="https://github.com/user-attachments/assets/b8e18fed-bfa2-4d2a-995b-f1f64d1aabd8" />

# VNC

Per fer servir VNC m'agrada utilitzar Remmina, un programari de connexió remota. S'instala amb:

<img width="715" height="99" alt="imatge" src="https://github.com/user-attachments/assets/8f206914-aaf3-4283-af33-8eacf2cf7f1a" />

També és necessari tindre un servidor VNC al que conectarse:

<img width="683" height="134" alt="imatge" src="https://github.com/user-attachments/assets/8c66679c-a914-4a47-8351-115640d3171c" />

Ara cal permetre la compartició de pantalla a la configuració local de la màquina:

<img width="710" height="298" alt="Captura de pantalla de 2026-04-24 12-02-13" src="https://github.com/user-attachments/assets/2ef92d7f-a43b-4d4d-a4ee-8d3c94823fae" />

Per últim, obrim Remmina i li donem a "Nova connexió" i introduïm les dades de la màquina a connectar-se.

<img width="960" height="661" alt="Captura de pantalla de 2026-04-24 12-06-02" src="https://github.com/user-attachments/assets/0f31b4fc-6b1d-429c-ba82-729442590162" />

<img width="1920" height="987" alt="imatge" src="https://github.com/user-attachments/assets/9986935c-f3b7-41ef-8f6e-2c0340f5b3da" />





