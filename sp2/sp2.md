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

GParted és una eina lliure per gestionar particions de disc amb una interfície gràfica senzilla.
Permet crear, redimensionar, moure i eliminar particions de manera segura en diversos sistemes de fitxers.


<img width="770" height="548" alt="imatge" src="https://github.com/user-attachments/assets/87667e81-af28-4447-915a-5939bb1093f4" />



# Comandes

Les comandes de terminal per formatar discos en Linux inclouen eines com **mkfs** (com *mkfs.ext4*, *mkfs.vfat*, *mkfs.ntfs*) i **fdisk** per crear o modificar particions abans de formatar-les.
El fitxer **/etc/fstab** defineix quines particions o sistemes de fitxers s’han de muntar automàticament en arrencar i amb quines opcions de muntatge.


<img width="736" height="716" alt="imatge" src="https://github.com/user-attachments/assets/076a1a81-adae-4dbb-8bc7-fe8bdd5e15d6" />

<img width="605" height="97" alt="imatge" src="https://github.com/user-attachments/assets/12398f23-809f-4ede-b745-45587f2d43a0" />

<img width="738" height="275" alt="imatge" src="https://github.com/user-attachments/assets/b0848ce1-2a0a-493a-ac61-d61e66222733" />

<img width="598" height="131" alt="imatge" src="https://github.com/user-attachments/assets/cea0c20b-7f32-4fae-99c5-97284b87167f" />

<img width="608" height="371" alt="imatge" src="https://github.com/user-attachments/assets/1251f90d-dc30-481e-a7a4-84c13ebfff42" />

<img width="670" height="147" alt="imatge" src="https://github.com/user-attachments/assets/ebdd0f13-994d-4d2a-bdf3-67700ac90c38" />

<img width="736" height="378" alt="imatge" src="https://github.com/user-attachments/assets/273be3b0-8633-4293-abbd-e1e1731698a0" />

<img width="444" height="124" alt="imatge" src="https://github.com/user-attachments/assets/a98b3c31-6334-48b3-848e-e25d7a6db6c1" />


### Còpies de seguretat i automatització de tasques

1- Teoria còpies de seguretat
Còpia completa: Es fa una còpia de tot el seleccionat, ens quedem fora de duptes però sont grans i lentes. Actualment les millors.
Còpia diferencial: A partir de la còpia completa, es resguarda la diferencia del contingut, afegint-se a la completa. Són ràpides i petites, però depenen de la còpia completa.
Còpia incremental: A partir de la còpia completa, també es resguarda la diferencia del contingut, però cada incremental es guarda a partir de l'anterior. Són més petites encara, però en cas de backup cal totes les incrementals acumulades.


2- Teoria comandes backups+
cp: Comanda bàsica de copiar, utilitzada en entorns locals. No és intel·ligent.
rsync: Crea sincronitzacions de carpetes, permet fer còpies en local i remot via SSH. És intel·ligent.
dd: "dd" no és per a fer còpies, és per a clonar particions o discos. No és intel·ligent.

3- Pràctica comandes backup
cp:
<img width="735" height="318" alt="imatge" src="https://github.com/user-attachments/assets/cbc42363-f93b-4fef-b264-082524218511" />
rsync:
<img width="743" height="416" alt="imatge" src="https://github.com/user-attachments/assets/78babdff-f23c-4151-a797-7702020c1557" />
dd:
<img width="739" height="223" alt="imatge" src="https://github.com/user-attachments/assets/113ff3b4-41ff-4ec6-99c2-5b423eec9b02" />


4- Pràctica programes backup
Deja-Dup
5- Teoria Automatització scripts, cron i anacron
Un script és un fitxer que serveix per automatizar tasques, poden ser simples o complexes i en diversos llenguatges.
<img width="736" height="198" alt="imatge" src="https://github.com/user-attachments/assets/fd883587-698d-4a35-a159-3909152294fe" />
<img width="583" height="102" alt="imatge" src="https://github.com/user-attachments/assets/71cc178c-89f1-4b1d-ac0c-a05cdd774679" />

<img width="720" height="186" alt="imatge" src="https://github.com/user-attachments/assets/89b4b9ba-8b05-4a5c-ad3c-dc68a91de26f" />
<img width="277" height="336" alt="imatge" src="https://github.com/user-attachments/assets/00cbad90-2836-44cf-a3ac-6d6cc78ce4fa" />

<img width="720" height="71" alt="imatge" src="https://github.com/user-attachments/assets/28120412-6904-4bec-acc9-40e16b59473d" />
<img width="719" height="132" alt="imatge" src="https://github.com/user-attachments/assets/07eeffd8-b49c-4a0e-8128-c9192acf4e7b" />
<img width="730" height="173" alt="imatge" src="https://github.com/user-attachments/assets/6e1a0b8d-e4bd-4834-af6a-9cafa8570850" />

Funciona:
<img width="730" height="173" alt="imatge" src="https://github.com/user-attachments/assets/78342194-476d-43a1-9272-29a4b3328be9" />


6- Pràctica automatització
6.1- cron
El cron s'utilitza normalment per automatizar tasques per a usuaris especifics en una data i hora concrets. Si en aquell moment l'ordinador està tancat, la tasca es perd.
<img width="734" height="484" alt="imatge" src="https://github.com/user-attachments/assets/f017fa13-8b67-45aa-aabb-9dd6d724aa30" />

Carpetes cron:
<img width="621" height="278" alt="imatge" src="https://github.com/user-attachments/assets/cd6f9835-4357-433a-a42f-7d1bdb94b6ab" />


6-2- anacron
Anacron és el mateix, però la tasca no es perd perqué anacron el recupera.
<img width="734" height="484" alt="imatge" src="https://github.com/user-attachments/assets/0370299f-7885-480f-a74b-400d68552140" />


Abans anaven per separat, però actualment treballen junts.

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


Podem borrar usuaris amb "deluser", però no borra els seus remanents. En canvi, "userdel -r" sí.

<img width="750" height="193" alt="imatge" src="https://github.com/user-attachments/assets/7281fd84-7029-4309-8260-a112802be516" />

Per bloquejar un usuari, es fa servir "usermod -L". Per tornar-ho a habilitar, es fa "usermod -U".

<img width="737" height="228" alt="imatge" src="https://github.com/user-attachments/assets/df735330-4185-4809-9c29-056d7aac635a" />

Creació de grups.

<img width="539" height="157" alt="imatge" src="https://github.com/user-attachments/assets/f6a4145d-e4c3-47bd-8c70-f665a9410a7e" />

Afegir usuaris a un grup:

<img width="511" height="185" alt="imatge" src="https://github.com/user-attachments/assets/eaebcebc-a7a3-42a3-9a0f-4481b542ed09" />

Llevar usuaris d'un grup:

<img width="511" height="150" alt="imatge" src="https://github.com/user-attachments/assets/fa2165e3-1c73-4dd2-a762-195fb303ae06" />

Canviar grup principal d'un usuari:

<img width="551" height="86" alt="imatge" src="https://github.com/user-attachments/assets/03fcb400-f743-4cbb-9703-5bf0c4dab415" />

Eliminem grups amb "groupdel", però en cas de que el grup sigui el principal d'un o més usuaris, no es podrà executar la comanda.

<img width="640" height="101" alt="imatge" src="https://github.com/user-attachments/assets/c856871f-9bf1-4ca7-8b92-77059410a318" />

Hi ha uns fitxers que ens permet personalitzar el comportament de les comandes "adduser" i "useradd". "adduser.conf" sols afecta a la comanda "adduser, "useradd" sols a la comanda "useradd" i "login.defs" a ambdues.

<img width="638" height="83" alt="imatge" src="https://github.com/user-attachments/assets/e9c3551a-f1b2-41b7-9068-3a382d3498f2" />

Exemples personals:

<img width="728" height="412" alt="imatge" src="https://github.com/user-attachments/assets/a8feba29-d38d-4cd9-b466-e5d50031befe" />

<img width="728" height="412" alt="imatge" src="https://github.com/user-attachments/assets/2beb3768-515c-49a7-ac13-c1289baeead3" />

<img width="728" height="412" alt="imatge" src="https://github.com/user-attachments/assets/3609dbee-1795-4bc4-85cf-475e0052a864" />


També, al crear amb "adduser", tot el que està a /etc/skel/ es copiarà a la carpeta personal de l'usuari. Amb això, farem un parell de proves.


Carpetes del /etc/skel:


<img width="364" height="211" alt="imatge" src="https://github.com/user-attachments/assets/cfec6b68-49d1-4715-9031-d77119fd87de" />



<img width="626" height="98" alt="imatge" src="https://github.com/user-attachments/assets/5c4c629c-8494-45f4-9377-a852ac6a0898" />

`.profile` carrega configuracions d’entorn quan inicies sessió, `.bashrc` defineix alias i funcions per a cada shell interactiu, i `.bash_logout` executa ordres en tancar la sessió.
I aquí uns exemples personals


<img width="742" height="302" alt="image" src="https://github.com/user-attachments/assets/e4ad8b31-d03e-4cf7-919c-72373690108d" />

<img width="739" height="186" alt="image" src="https://github.com/user-attachments/assets/96735e69-11eb-42d1-b6cd-0545a3c77810" />


<img width="745" height="225" alt="image" src="https://github.com/user-attachments/assets/baac8ea6-c6f7-4e62-9e9b-200656f2276b" />

## Gestió de permisos

Preparo l'entorn per als següents pasos:

<img width="620" height="493" alt="imatge" src="https://github.com/user-attachments/assets/55edde1d-f153-4a1a-b271-78730fb095cf" />
<img width="512" height="278" alt="imatge" src="https://github.com/user-attachments/assets/efef0b84-6fc9-4f54-89fc-0a7b9b1a545e" />

<img width="618" height="295" alt="imatge" src="https://github.com/user-attachments/assets/fa57ca30-8741-4a9e-9bcc-ea22ef0dd910" />

<img width="612" height="277" alt="imatge" src="https://github.com/user-attachments/assets/5bcdb0ff-fb90-4db7-8ab0-0c698a7ba984" />

<img width="727" height="313" alt="imatge" src="https://github.com/user-attachments/assets/303c0aba-697a-401b-bf49-06860e420672" />

## ACL

<img width="697" height="388" alt="imatge" src="https://github.com/user-attachments/assets/bd81088e-dbcb-43e1-a5cb-7c3f0e368145" />

<img width="706" height="423" alt="imatge" src="https://github.com/user-attachments/assets/8cc2dede-bb87-4642-8cf3-7c78905d3bfb" />

<img width="461" height="164" alt="imatge" src="https://github.com/user-attachments/assets/c6d29ddc-0841-48f1-b48f-5452d5555a72" />

<img width="731" height="420" alt="imatge" src="https://github.com/user-attachments/assets/3a0ac154-6e5a-451f-8ddd-f23459993697" />


### Gestió de procesos

