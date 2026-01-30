---
layout: default
title: "A1. Sprint 3: Gestió de Dominis i Accessos"
---

# Instal·lació de dominis LDAP i unir client al domini

<img width="898" height="583" alt="imatge" src="https://github.com/user-attachments/assets/5a4439cf-12b7-491b-9c81-95ccbc978bfa" />

<img width="898" height="583" alt="imatge" src="https://github.com/user-attachments/assets/c3629680-e613-4e83-ae4b-386a632b6219" />

Un servidor ha tenir una IP fixa per ser localitzat en tot moment.

<img width="623" height="532" alt="imatge" src="https://github.com/user-attachments/assets/e7576646-db5e-4262-80cc-8de3235557b0" />

<img width="733" height="151" alt="imatge" src="https://github.com/user-attachments/assets/c48d0015-7783-47a6-b072-7f4ace3bec05" />

<img width="733" height="151" alt="imatge" src="https://github.com/user-attachments/assets/43658f82-c309-4db8-b084-d6a76a0bbe82" />

Després d'un update, instal·larem el paquets de l'LDAP mitjançant apt.

<img width="735" height="88" alt="imatge" src="https://github.com/user-attachments/assets/b63da425-1b43-4f94-9674-69e860bf3161" />


<img width="740" height="492" alt="imatge" src="https://github.com/user-attachments/assets/4de79480-4b19-49dc-8d1d-94e60d5d238d" />

<img width="731" height="455" alt="imatge" src="https://github.com/user-attachments/assets/9f6a93c4-db8f-4725-a69b-d0ee6a18c95b" />

<img width="731" height="455" alt="imatge" src="https://github.com/user-attachments/assets/b81f4668-2b4a-44b2-b821-b2472ff39ffd" />

<img width="731" height="455" alt="imatge" src="https://github.com/user-attachments/assets/abc17124-7c6c-4e02-98c7-075115398245" />

<img width="731" height="455" alt="imatge" src="https://github.com/user-attachments/assets/832f2d37-e46c-4bf3-b3ce-78bc1860a7f8" />


<img width="731" height="455" alt="imatge" src="https://github.com/user-attachments/assets/1d6fd437-8db3-4669-a507-be66a850f3cb" />

<img width="761" height="326" alt="imatge" src="https://github.com/user-attachments/assets/b00463ac-a7c8-4436-8432-e3f43c6bba47" />

<img width="604" height="409" alt="imatge" src="https://github.com/user-attachments/assets/4334ad2f-f0b7-4981-aa52-1508bf74aa47" />

<img width="691" height="156" alt="imatge" src="https://github.com/user-attachments/assets/e99c6f66-3b59-4fa5-a7a7-96f168b048ef" />

<img width="715" height="465" alt="imatge" src="https://github.com/user-attachments/assets/76712d86-7722-4f3a-8ddd-7db095f84e60" />

<img width="715" height="465" alt="imatge" src="https://github.com/user-attachments/assets/6a401b44-f0c5-4286-8cf3-0c4c97991c55" />

<img width="715" height="465" alt="imatge" src="https://github.com/user-attachments/assets/e45567e9-84c7-400e-8f86-26a06224393b" />

<img width="715" height="465" alt="imatge" src="https://github.com/user-attachments/assets/71483c35-2045-430b-8688-18be04b7b815" />

<img width="715" height="465" alt="imatge" src="https://github.com/user-attachments/assets/6abea938-c91a-4b61-908c-3874b4541601" />

<img width="715" height="465" alt="imatge" src="https://github.com/user-attachments/assets/fd5eb25f-8c85-43dd-87c7-757dd31cc95b" />

<img width="715" height="465" alt="imatge" src="https://github.com/user-attachments/assets/db198ebf-cab3-42ba-b6f9-61fd78faf134" />

<img width="715" height="465" alt="imatge" src="https://github.com/user-attachments/assets/cd6b1bf9-f163-4009-8926-559bd462a966" />

<img width="715" height="465" alt="imatge" src="https://github.com/user-attachments/assets/70114c86-83d3-4042-97dd-a8c1e180c42e" />

<img width="715" height="465" alt="imatge" src="https://github.com/user-attachments/assets/4d187f11-f726-4aa5-8f5a-ba5264f1938b" />

<img width="715" height="465" alt="imatge" src="https://github.com/user-attachments/assets/a0c92504-4388-4c6c-8fd8-7dd13670629c" />

<img width="715" height="465" alt="imatge" src="https://github.com/user-attachments/assets/f6e354a6-3f6f-4230-9578-47059bc44970" />

<img width="715" height="465" alt="imatge" src="https://github.com/user-attachments/assets/11ec6822-ea6d-4ccf-a8d8-2c2341e9c71b" />

<img width="715" height="465" alt="imatge" src="https://github.com/user-attachments/assets/5a78eace-6702-43cc-8603-b4f2f0653c2e" />

<img width="572" height="210" alt="imatge" src="https://github.com/user-attachments/assets/14bd92b0-05ed-4934-9d04-93903588e115" />

<img width="572" height="210" alt="imatge" src="https://github.com/user-attachments/assets/5c226454-8c32-4537-9aed-530a99505943" />

<img width="572" height="210" alt="imatge" src="https://github.com/user-attachments/assets/2de68de7-0d1b-4238-9bbf-3f5e6dcf99bf" />


Exercicis:
### [PDF amb les comandes i resultats](sp3/exLDAP.pdf)


# Servidor samba i NFS

Serveixen per a compartir fitxers o recursos, a més, samba et deixa compartir impresores i fer la autenticació al LDAP. NFS ho fa a partir d'IP

## Samba

<img width="486" height="100" alt="imatge" src="https://github.com/user-attachments/assets/51510faf-ea3a-4ecd-b7c9-c878db8b9e01" />

<img width="535" height="130" alt="imatge" src="https://github.com/user-attachments/assets/1753321b-a82e-4944-acc6-c6190dd434c6" />

<img width="456" height="240" alt="imatge" src="https://github.com/user-attachments/assets/eb0a388c-f00f-45d7-8249-46e04400e5b4" />

<img width="456" height="240" alt="imatge" src="https://github.com/user-attachments/assets/5658e36c-18ff-4c8e-982b-8df30b482582" />

<img width="734" height="493" alt="imatge" src="https://github.com/user-attachments/assets/109da6cc-b2c7-4378-af1e-474c68d8506e" />

<img width="507" height="88" alt="imatge" src="https://github.com/user-attachments/assets/1505a6fd-4f11-44b3-97c0-d77f44a9d83e" />

<img width="699" height="500" alt="imatge" src="https://github.com/user-attachments/assets/c4274bdf-2a4f-4beb-916d-fe6735b620de" />

<img width="666" height="226" alt="imatge" src="https://github.com/user-attachments/assets/af30fb66-8f5e-4077-961e-c6aecdc9bc83" />


<img width="616" height="203" alt="imatge" src="https://github.com/user-attachments/assets/3c525f0c-3a7d-4d35-8a97-0c1daa743ff2" />

<img width="695" height="486" alt="imatge" src="https://github.com/user-attachments/assets/0d4ae0f0-6153-48bb-996c-285c2e4ed99e" />

<img width="695" height="486" alt="imatge" src="https://github.com/user-attachments/assets/3b4bb10c-b3bd-481a-9bf5-17b8f149b747" />

<img width="695" height="486" alt="imatge" src="https://github.com/user-attachments/assets/c8df8cb8-0c7d-4726-88f9-06fd3ab3eaac" />

Com es denega l'accés, torna a la pantalla sense infomació d'usuari, és a dir, anonim.

<img width="695" height="486" alt="imatge" src="https://github.com/user-attachments/assets/1f38fcb3-fa48-4bdc-abbf-d4f48693e33c" />





## NFS


