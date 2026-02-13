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

### Server

<img width="716" height="140" alt="imatge" src="https://github.com/user-attachments/assets/8308b680-d94b-4df6-a506-a637538e2c50" />


<img width="753" height="227" alt="imatge" src="https://github.com/user-attachments/assets/ae93e353-9073-4ab1-8d70-1fcd8a8ce419" />

<img width="721" height="160" alt="imatge" src="https://github.com/user-attachments/assets/755a118e-9dde-4aaf-baa2-ebcdebeedfa0" />

<img width="727" height="345" alt="imatge" src="https://github.com/user-attachments/assets/0d7a452d-e39a-4be0-b72d-f04b4caa55d3" />


### Client

<img width="703" height="135" alt="imatge" src="https://github.com/user-attachments/assets/8ac68edc-2dc0-4eef-8ae1-1a8d6498b96f" />

<img width="614" height="132" alt="imatge" src="https://github.com/user-attachments/assets/75ef5498-389d-4250-8846-25dac8cddc46" />

<img width="1391" height="366" alt="imatge" src="https://github.com/user-attachments/assets/21949b89-5133-4045-8164-44a7785d8b79" />

<img width="406" height="102" alt="imatge" src="https://github.com/user-attachments/assets/060f98cb-f581-4623-a07a-9a92d44d39e7" />

<img width="357" height="130" alt="imatge" src="https://github.com/user-attachments/assets/8f50d59e-21a9-44a4-9407-f7e192015319" />

<img width="672" height="134" alt="imatge" src="https://github.com/user-attachments/assets/843a6f07-754f-4744-baf8-21fb146a4341" />

<img width="373" height="85" alt="imatge" src="https://github.com/user-attachments/assets/bf23c007-f11a-4760-9780-22584f50edfa" />


### Amb usuaris

<img width="407" height="104" alt="imatge" src="https://github.com/user-attachments/assets/4bedd9cf-bdcd-431c-88ca-ba7cfbf723a4" />


<img width="669" height="139" alt="imatge" src="https://github.com/user-attachments/assets/85374d50-de66-4299-bc36-890e22b52636" />


<img width="736" height="496" alt="imatge" src="https://github.com/user-attachments/assets/aee27afe-1ff9-4ef0-9778-1bacbd2a41b8" />

<img width="753" height="113" alt="imatge" src="https://github.com/user-attachments/assets/fa9be27e-fa5a-429e-9f71-1c0d9cff6c9d" />


<img width="400" height="87" alt="imatge" src="https://github.com/user-attachments/assets/8acd88fb-cc5e-4694-bedc-ad5c12a430d3" />


<img width="472" height="143" alt="imatge" src="https://github.com/user-attachments/assets/062d4e85-1f81-46a8-98d2-1369017f9544" />


## NFS Windows

<img width="865" height="385" alt="imatge" src="https://github.com/user-attachments/assets/a2f8845a-efd6-44ab-83f8-ec04f37ebb63" />

<img width="659" height="544" alt="imatge" src="https://github.com/user-attachments/assets/ae6106d6-e0eb-497b-915d-ca759f7c4b8e" />

<img width="1225" height="694" alt="imatge" src="https://github.com/user-attachments/assets/9cc0c27c-34e0-49d0-9005-97edc3ea58c2" />

<img width="1225" height="694" alt="imatge" src="https://github.com/user-attachments/assets/ebd12c17-d485-40ff-8f40-f3b15f91a07a" />
