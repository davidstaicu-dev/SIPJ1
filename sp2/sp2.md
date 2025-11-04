---
layout: default
title: "A1. Sprint 2: Gestió de la Informació del Sistema i Administració"
---

### Sistemes de fitxers i particions

## Mida del sector

Un sector és la unitat mínima física on es guarden les dades al disc. Aquella mida no es modificar.

<img width="697" height="192" alt="imatge" src="https://github.com/user-attachments/assets/da4f685e-6ece-4f0b-b912-65892a7577c1" />

## Mida del block

Un block és la unitat mínima llògica on es guarden les dades a nivell sistema operatiu. Aquesta mida es de 4096 bytes. Es pot modificar al moment de formatar.

<img width="467" height="116" alt="imatge" src="https://github.com/user-attachments/assets/9334e800-f2d9-4ad9-9722-99f3e54c92c5" />

<img width="263" height="230" alt="imatge" src="https://github.com/user-attachments/assets/97f87195-b38d-41f9-9a43-98552a1ee89a" />


## Fragmentació interna

Al ocuparar sempre blocs de 4096 bytes, si es tracta d'un fitxer més petit, es desaprofita espai. La fragmentació interna tracta en no desaprofitar-ho.

## Fragmentació externa

La fragmentaicó externa ocurreix quan, a mesura que es treballa amb el sistema operatiu, els fitxers ja no es van guardant en blocs continus de memoria. Així que el rendiment baixa entre altres.

Windows té el Desfragmentador de disc. A Linux, es sol dir que és tan bo que no fa falta un desfragmentador, encara que hi té.

<img width="824" height="439" alt="imatge" src="https://github.com/user-attachments/assets/e41408c4-3181-4b02-9512-ea0e70af9ba6" />

<img width="811" height="425" alt="imatge" src="https://github.com/user-attachments/assets/17394712-23fc-4708-b1c2-e921e3146fd0" />

## Tipus de sistemes de fitxers

Hi ha molts d'ells. Els més coneguts són: NTFS, EXT4, FAT32.

Cadascun té moltes caracteristiques, entre elles: Sistema operatiu que pot accedir, mida dels blocs, mida dels fitxers, nom dels fitxers...

## Tipus de formateig

- Alt nivell: No se esborra les dades, més bé el sistema de fitxers. Es podrien recuperar del dades.
- Mig nivell: Com el d'alt nivell, però marca sectors a nivell de disc defectuosos, indicant falles.
- Baix nivell: Borra tant el sistema de fitxers com els arxius.

## Particions/volumns

Una partició es una separació del disc a nivell físic.
Un volumn és com una capa d'abstracció que es fica per damunt de les particions.

<img width="680" height="422" alt="imatge" src="https://github.com/user-attachments/assets/f381f8bb-5928-4545-b321-39ba4afc94af" />

<img width="630" height="135" alt="imatge" src="https://github.com/user-attachments/assets/3ad9a39d-5646-4ef0-9eae-16aa99a6a284" />


# Gparted

<img width="770" height="548" alt="imatge" src="https://github.com/user-attachments/assets/87667e81-af28-4447-915a-5939bb1093f4" />



# Comandes

<img width="736" height="716" alt="imatge" src="https://github.com/user-attachments/assets/076a1a81-adae-4dbb-8bc7-fe8bdd5e15d6" />

<img width="605" height="97" alt="imatge" src="https://github.com/user-attachments/assets/12398f23-809f-4ede-b745-45587f2d43a0" />

<img width="738" height="275" alt="imatge" src="https://github.com/user-attachments/assets/b0848ce1-2a0a-493a-ac61-d61e66222733" />

<img width="598" height="131" alt="imatge" src="https://github.com/user-attachments/assets/cea0c20b-7f32-4fae-99c5-97284b87167f" />

<img width="608" height="371" alt="imatge" src="https://github.com/user-attachments/assets/1251f90d-dc30-481e-a7a4-84c13ebfff42" />

<img width="670" height="147" alt="imatge" src="https://github.com/user-attachments/assets/ebdd0f13-994d-4d2a-bdf3-67700ac90c38" />

<img width="736" height="378" alt="imatge" src="https://github.com/user-attachments/assets/273be3b0-8633-4293-abbd-e1e1731698a0" />

<img width="444" height="124" alt="imatge" src="https://github.com/user-attachments/assets/a98b3c31-6334-48b3-848e-e25d7a6db6c1" />


### Còpies de seguretat i automatització de tasques

### Gestió d'usuaris, grups i permisos

Al fitxer "passwd" a la carpeta "etc" mostra tots els usuaris del sistema.

<img width="738" height="494" alt="imatge" src="https://github.com/user-attachments/assets/0080afcb-9ac0-442a-8802-afdf967ab39a" />

Al fitxer "group" els grups que té el sistema.

<img width="738" height="494" alt="imatge" src="https://github.com/user-attachments/assets/0f2a7289-6812-4948-8705-199eaccee51a" />

Al fitxer "shadow" es troben les contrasenyes dels usaris encriptades.

<img width="738" height="494" alt="imatge" src="https://github.com/user-attachments/assets/f657898b-1b5e-4c26-83ee-01826408698b" />

Al fitxer "gshadow" es veuen els administradors de cada grup.

<img width="760" height="500" alt="imatge" src="https://github.com/user-attachments/assets/e9a51286-174a-4c2f-bc2d-d53012b68e34" />


Crearem un usuari nom "xavi" d'exemple, se li crearà una home automaticament, pero sense contingut (Descarregues, Imatges, Documents...). Per a que apareguen, cal entrar per primera vegada a l'usari, després ja sortirà.

<img width="783" height="186" alt="imatge" src="https://github.com/user-attachments/assets/cec39fd1-1f6d-4981-9492-5b55b6aed5d2" />

També podem fer servir "useradd", però caldrà introduir els demés parametres amb comandes també.
<img width="735" height="413" alt="imatge" src="https://github.com/user-attachments/assets/64798ca3-e9f7-41cc-ad96-33028a9ca220" />

<img width="599" height="133" alt="imatge" src="https://github.com/user-attachments/assets/803b0125-0c49-4014-b032-ded34bd61e90" />


### Gestió de procesos

