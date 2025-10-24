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

## Instantanies

Afegim un nou disc virtual

<img width="708" height="405" alt="image" src="https://github.com/user-attachments/assets/1b52e4c0-4210-454c-91cc-b4489fecb451" />

Amb l’eina «fdisk», accedim a aquest nou disc (sdb) per formatar-ho a ext4 (sistema de fitxer d’ubuntu). Crearem una partició amb tot l’espai i la formatarem.

<img width="730" height="289" alt="image" src="https://github.com/user-attachments/assets/566f3cd8-aa72-4cac-97aa-6c88f6ccdcc0" />

<img width="756" height="268" alt="image" src="https://github.com/user-attachments/assets/f5014c7e-67dd-4cde-bf6f-04380db9ec30" />

<img width="719" height="210" alt="image" src="https://github.com/user-attachments/assets/a55a994c-b0b9-4986-8def-ec461fd76c38" />

<img width="749" height="322" alt="image" src="https://github.com/user-attachments/assets/8047941e-7e04-46a9-8ec0-9c5d0377c541" />

Després instal·lem «timeshift	», un programari per realitzar instantànies.

<img width="514" height="115" alt="image" src="https://github.com/user-attachments/assets/db052fa3-1742-4a06-b35c-7feb6dc70f51" />

<img width="143" height="165" alt="image" src="https://github.com/user-attachments/assets/6bf58f38-512b-4db6-873d-485071cacff9" />

Hi creem uns quants arxius que després esborrarem per comprovar que es recuperen.

<img width="566" height="210" alt="image" src="https://github.com/user-attachments/assets/27a267ac-2247-4560-96cf-d14de1011fa8" />

El següent és configurar timeshift, com el tipus, lloc (ho ficarem tot al segon disc d’abans), i les carpetes a assegurar.

<img width="592" height="263" alt="image" src="https://github.com/user-attachments/assets/dbae4f2b-de92-41d2-852b-2dcbb1741679" />

<img width="593" height="285" alt="image" src="https://github.com/user-attachments/assets/00f252c1-48d1-4f7a-9663-671daf72b913" />

<img width="789" height="368" alt="image" src="https://github.com/user-attachments/assets/67a49565-e99e-4412-8da2-9d0d607561ef" />

Ara ho esborrem i després de fer la recuperació, tornen a estar els fitxers.

<img width="720" height="181" alt="image" src="https://github.com/user-attachments/assets/f8bec17c-a550-4954-b549-6d0a33c162a4" />

<img width="737" height="175" alt="image" src="https://github.com/user-attachments/assets/d100358d-82a9-4a73-90ad-7ac4c852d7c0" />


## Particions i punts de restauració







## Configuració bàsica de la xarxa

Deixarem la màquina en Adaptador pont perquè la xarxa la identifiqui com un dispositiu independent. 

<img width="1018" height="617" alt="image" src="https://github.com/user-attachments/assets/44b7a5d8-1e71-4f55-8c18-682e69ca62c8" />

Prova de connexió.

<img width="735" height="236" alt="image" src="https://github.com/user-attachments/assets/b16ea57b-0741-4fb5-b453-432cf8fd070a" />

<img width="710" height="208" alt="image" src="https://github.com/user-attachments/assets/b58a4e8a-2ea5-48f2-8477-ecaf4dc2fa16" />

<img width="601" height="218" alt="image" src="https://github.com/user-attachments/assets/b79260cc-203f-49ab-af7e-408378186fb0" />

Modificació del fitxer netplan per a IP estàtica.

<img width="737" height="493" alt="image" src="https://github.com/user-attachments/assets/43d59cd8-26a5-456b-b68a-61ec75463cc4" />

Prova de connexió.

<img width="730" height="311" alt="image" src="https://github.com/user-attachments/assets/b1382b03-8107-43cc-8d2c-31c656822f5d" />

<img width="741" height="610" alt="image" src="https://github.com/user-attachments/assets/a3f0c55a-a570-4667-9518-e0eee52aa142" />


## Comandes generals i instal·lació d'aplicacions

<img width="726" height="178" alt="image" src="https://github.com/user-attachments/assets/dafa2fbe-1131-4f2d-ae1b-da9654b1b412" />

