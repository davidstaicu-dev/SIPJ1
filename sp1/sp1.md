---
layout: default
title: "A1. Sprint 1: Instal·lació i Configuració Inicial"
---

## Virtualització i instal·lació del SO Ubuntu
### Llicenciament
Canonical, l'equip darrere d'Ubuntu, ja té públicada a la seva web la [llicencia detallada](https://canonical.com/legal/terms-and-policies). Tot i així, dins del sistema operatiu es troben diverses llicencies.

<img width="603" height="148" alt="image" src="https://github.com/user-attachments/assets/c4b89fe4-e99d-4406-8b59-01b711172174" />

### Particions

<img width="876" height="534" alt="image" src="https://github.com/user-attachments/assets/04649a78-f22a-410b-bc2f-7f7e13d445a5" />

### Ubuntu Instal·lat
<img width="1920" height="1049" alt="image" src="https://github.com/user-attachments/assets/47b8434d-7c11-4ab7-906b-b0fcd16f3da8" />


## Instal·lació duals i Gestors d'arrencada

### Hablitem EFI
<img width="869" height="587" alt="image" src="https://github.com/user-attachments/assets/02e44abd-6bb7-4504-9e23-f9481998b38b" />

### Posem la ISO de Windows 10
<img width="869" height="587" alt="image" src="https://github.com/user-attachments/assets/ae2de6eb-0f21-4773-a367-53deb035e209" />

### Particions
<img width="869" height="587" alt="image" src="https://github.com/user-attachments/assets/f274ede7-2fd5-476c-93e0-e3e0a93c288b" />

D'alguna manera, el gestor d'arranc d'Ubuntu no ha petat. Llavors he pogut tornar a Ubuntu. Però ara com puc tornar a Windows? Cal instal·lar el GRUB, per triar entre Windows o Ubuntu. Sols cal aquesta comanda:
<img width="742" height="305" alt="image" src="https://github.com/user-attachments/assets/89ccc0af-1ceb-4203-a427-4810fc69d8a5" />

És possible que s'hagi de modificar el fitxer /etc/default/grub per posar el TIMEOUT diferent a 0. A més de comentar la segona linia i afegir "GRUB_DISABLE_OS_PROBER=false" en cas de no estar.

<img width="742" height="305" alt="image" src="https://github.com/user-attachments/assets/b154ff85-cf21-4918-a2b7-f1dc2e992f6e" />

Després per aplicar els canvis cal introduir altra comanda:
<img width="742" height="305" alt="image" src="https://github.com/user-attachments/assets/b77502c5-ac0b-4992-b9f1-a40a2cbfa898" />

En reiniciar es veu el GRUB:

<img width="1017" height="268" alt="image" src="https://github.com/user-attachments/assets/37f9b87f-5dc4-4cde-9a9b-4b8fd69cec7f" />


## Particions i punts de restauració
## Configuració bàsica de la xarxa
## Comandes generals i instal·lació d'aplicacions
