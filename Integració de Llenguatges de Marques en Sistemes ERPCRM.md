# Tasca de Recerca: Integració de Llenguatges de Marques en Sistemes ERP/CRM

En l’actualitat, les empreses utilitzen sistemes ERP i CRM per centralitzar la gestió de les seves dades. Aquests sistemes no funcionen de manera aïllada, sinó que sovint s’han d’integrar amb bancs, botigues online, proveïdors, plataformes logístiques o administracions públiques. Per aquest motiu, els llenguatges de marques i formats d’intercanvi de dades, com XML, JSON, CSV o EDI, tenen un paper essencial en la comunicació entre sistemes.

## 1. Fonaments de Sistemes Empresarials

### Què és un ERP?

Un **ERP** (*Enterprise Resource Planning*) és un sistema de gestió empresarial que integra diferents àrees d’una empresa en una mateixa plataforma: comptabilitat, compres, vendes, magatzem, recursos humans, producció, facturació, etc. La seva funció principal és centralitzar la informació perquè tots els departaments treballin amb les mateixes dades.

<img width="1024" height="316" alt="image" src="https://github.com/user-attachments/assets/bdf95046-aa92-4c43-9f6b-eef0c1cd0228" />

### Què és un CRM?

Un **CRM** (*Customer Relationship Management*) és un sistema orientat a gestionar la relació amb els clients. Serveix per controlar contactes, oportunitats de venda, seguiment comercial, incidències, campanyes de màrqueting i atenció al client.

<img width="1000" height="1000" alt="image" src="https://github.com/user-attachments/assets/2b678a01-db99-4499-bdf9-fb7bee9d1958" />

##  Comparativa entre ERP i CRM

Tot i que els sistemes ERP i CRM poden estar connectats dins d’una mateixa empresa, no tenen exactament la mateixa funció. L’ERP se centra sobretot en la gestió interna de l’empresa, mentre que el CRM està més enfocat en la relació amb els clients.

| Aspecte | ERP | CRM |
|---|---|---|
| Significat | *Enterprise Resource Planning* | *Customer Relationship Management* |
| Objectiu principal | Gestionar i integrar els processos interns de l’empresa | Gestionar la relació amb els clients |
| Àrees principals | Comptabilitat, compres, vendes, magatzem, producció, recursos humans i facturació | Vendes, màrqueting, atenció al client i seguiment comercial |
| Tipus de dades que gestiona | Productes, factures, proveïdors, estoc, nòmines, comandes i comptabilitat | Clients, contactes, oportunitats de venda, incidències i campanyes |
| Exemple d’ús | Controlar l’estoc d’un producte i generar una factura | Registrar una trucada amb un client i fer seguiment d’una oportunitat de venda |
| Departaments que l’utilitzen | Administració, finances, logística, producció, compres i direcció | Equip comercial, màrqueting i atenció al client |
| Benefici principal | Millora l’organització interna i evita duplicar dades | Millora la comunicació amb els clients i ajuda a augmentar les vendes |
| Exemples de programari | Odoo, ERPNext, SAP, Microsoft Dynamics 365, Oracle NetSuite | SuiteCRM, Odoo CRM, Salesforce, HubSpot CRM, Microsoft Dynamics 365 Sales |

### Explicació tipo resum

Un **ERP** ajuda l’empresa a organitzar els seus recursos interns. Per exemple, quan es ven un producte, l’ERP pot actualitzar automàticament l’estoc, generar la factura i registrar el moviment comptable.

Un **CRM**, en canvi, ajuda a gestionar la relació amb els clients. Per exemple, permet guardar les dades d’un client, veure quines compres ha fet, registrar incidències o programar accions comercials.

Per tant, es podria dir que l’ERP mira més cap a l’interior de l’empresa, mentre que el CRM mira més cap a l’exterior, especialment cap als clients.

##  Exemples de programari ERP i CRM

A continuació es mostren alguns exemples de sistemes ERP i CRM, diferenciant entre programari lliure (*Open Source*) i programari propietari.

### Exemples d'ERP

| Tipus de programari | Exemple | Descripció breu |
|---|---|---|
| Open Source | Odoo Community | ERP modular amb aplicacions de vendes, compres, inventari, facturació i CRM. |
| Open Source | ERPNext | ERP de codi obert orientat a petites i mitjanes empreses. |
| Open Source | Dolibarr | ERP i CRM lliure, senzill i utilitzat per gestionar clients, factures, productes i projectes. |
| Propietari | SAP S/4HANA | ERP empresarial molt utilitzat en grans empreses. |
| Propietari | Microsoft Dynamics 365 | Plataforma empresarial de Microsoft amb funcions ERP i CRM. |
| Propietari | Oracle NetSuite | ERP al núvol orientat a la gestió empresarial integral. |

### Exemples de CRM

| Tipus de programari | Exemple | Descripció breu |
|---|---|---|
| Open Source | SuiteCRM | CRM lliure per gestionar clients, vendes, campanyes i incidències. |
| Open Source | EspoCRM | CRM de codi obert per gestionar contactes, empreses i oportunitats comercials. |
| Open Source | Odoo CRM Community | Mòdul CRM d’Odoo per gestionar oportunitats, clients i activitats comercials. |
| Propietari | Salesforce | Un dels CRM comercials més utilitzats a nivell mundial. |
| Propietari | HubSpot CRM | CRM propietari molt utilitzat en vendes, màrqueting i atenció al client. |
| Propietari | Microsoft Dynamics 365 Sales | CRM de Microsoft orientat a la gestió comercial i relació amb clients. |

### Explicació breu

Els sistemes **Open Source** permeten accedir al codi font i, en molts casos, adaptar el programa a les necessitats de l’empresa. Això pot ser molt útil per a empreses que volen personalitzar el sistema o reduir costos de llicències.

Els sistemes **propietaris**, en canvi, solen requerir el pagament de llicències o subscripcions. Normalment ofereixen suport professional, actualitzacions gestionades pel proveïdor i una infraestructura més orientada a grans empreses.


### Instal·lació On-premise i SaaS

<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/0e1842f9-2e7a-4c3c-8a6d-cb52a62d184e" />

Una instal·lació **On-premise** significa que el programari s’instal·la en servidors propis de l’empresa. L’empresa és responsable del manteniment, les còpies de seguretat, la seguretat, les actualitzacions i la infraestructura.

En canvi, una solució **SaaS o Cloud** funciona al núvol. L’empresa accedeix al sistema mitjançant Internet i normalment paga una subscripció. El proveïdor s’encarrega dels servidors, les actualitzacions i part de la seguretat. Per exemple, moltes empreses utilitzen Odoo, Salesforce o Microsoft Dynamics 365 en modalitat SaaS.

---

## 2. El paper de l’XML i JSON en l’intercanvi de dades

### Web Services i APIs

Els **Web Services** o **APIs** són mecanismes que permeten que dues aplicacions diferents es comuniquin entre elles. Per exemple, un ERP pot enviar dades de facturació a una gestoria, rebre comandes d’una botiga online o consultar l’estat d’un enviament amb una empresa logística.

Els formats **JSON** i **XML** s’utilitzen per estructurar aquestes dades de manera que siguin llegibles per diferents sistemes.

Per exemple, una botiga online pot enviar una comanda a l’ERP en format JSON. L’ERP rep la informació del client, els productes, les quantitats i l’import total, i automàticament pot crear una comanda de venda. També pot passar a l’inrevés: l’ERP pot exportar una factura en XML perquè una administració pública o una altra plataforma la pugui llegir.

JSON és molt habitual en APIs modernes perquè és més lleuger i fàcil de treballar amb aplicacions web. XML, en canvi, continua sent molt important en entorns més formals o regulats, com la facturació electrònica, alguns serveis bancaris o intercanvis amb administracions públiques.

#### Demostracio Real de com seria:
Primer he creat les carpetes per posar dins els .py

<img width="405" height="139" alt="image" src="https://github.com/user-attachments/assets/09cd9912-5ea3-463d-836f-c14f2dc21e6a" />

Tot seguit he creat l'aplicacio externa que rep les dades amb aquest codi

<img width="703" height="846" alt="image" src="https://github.com/user-attachments/assets/05f912c3-3875-4f52-83e4-c9a8ff90f1dd" />

Despres he executat la api externa

<img width="478" height="94" alt="image" src="https://github.com/user-attachments/assets/1d50553b-c4e3-47c0-9940-cbc073c753dc" />

Ara he obert una segona terminal per enviar dades json 

<img width="556" height="308" alt="image" src="https://github.com/user-attachments/assets/2262e198-6ded-4196-b085-62c6ca8b8e5d" />

A la terminal on esta la API oberta es veu com a la imatge

<img width="632" height="236" alt="image" src="https://github.com/user-attachments/assets/63449b70-cb05-4fe8-8f34-a8de6ac447b3" />

Això demostra que una aplicació externa pot rebre dades d’un ERP en format JSON.

Ara fare el mateix pero amb XML

<img width="429" height="263" alt="image" src="https://github.com/user-attachments/assets/5f259d02-6dd4-4b04-9f8a-5a45454be486" />

I a la terminal de l'API es veu com a la imatge:

<img width="628" height="395" alt="image" src="https://github.com/user-attachments/assets/0008de84-9459-4817-ab5a-4f636da5f9e6" />

En tots dos casos, les dades viatgen des de l’ERP fins a l’aplicació externa mitjançant una API. La diferència principal és la manera com s’estructuren les dades: JSON utilitza claus i valors, mentre que XML utilitza etiquetes.

Aquesta pràctica mostra que els formats JSON i XML serveixen perquè sistemes diferents puguin intercanviar informació de manera automàtica. En un cas real, aquest procés podria servir per enviar factures, comandes, dades de clients o informació d’estoc entre un ERP, una botiga online, una empresa logística o una administració pública.

### Què és EDI?

<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/bfc4576d-c41f-45b6-bffb-c59665cdf787" />

L’**EDI** (*Electronic Data Interchange*) és l’intercanvi electrònic de documents comercials entre empreses seguint formats estandarditzats. Pot servir per enviar comandes, albarans, factures, avisos d’expedició o confirmacions de recepció sense haver d’introduir les dades manualment.

Encara té molta rellevància en el sector logístic i en la cadena de subministrament, perquè permet automatitzar la comunicació entre fabricants, proveïdors, magatzems, distribuïdors i clients. Encara avui moltes empreses utilitzen estàndards EDI per automatitzar transaccions comercials entre sistemes.

## Exemple real d’empresa que utilitza EDI: Walmart

Un exemple real d’empresa que utilitza EDI és **Walmart**, una de les cadenes de distribució i venda al detall més grans del món.

<img width="1000" height="800" alt="image" src="https://github.com/user-attachments/assets/3f7c2144-9739-4347-8875-06c1a83ad756" />

Walmart utilitza EDI per comunicar-se amb els seus proveïdors i intercanviar documents comercials de manera automàtica. Segons la documentació per a proveïdors de Walmart, els venedors poden utilitzar una interfície EDI per transferir dades cap a Walmart.com i des de Walmart.com. Aquest sistema permet enviar i rebre informació sense haver d’introduir manualment les dades en cada plataforma.

Alguns documents habituals que es poden intercanviar mitjançant EDI són:

| Document EDI | Nom del document | Funció |
|---|---|---|
| EDI 850 | Purchase Order | Walmart envia una comanda de compra al proveïdor. |
| EDI 855 | Purchase Order Acknowledgment | El proveïdor confirma si accepta o pot complir la comanda. |
| EDI 856 | Advance Ship Notice | El proveïdor informa del contingut i detalls de l’enviament abans que arribi. |
| EDI 810 | Invoice | El proveïdor envia la factura electrònica a Walmart. |
| EDI 846 | Inventory Feed | El proveïdor informa de l’estoc disponible. |

### Exemple de funcionament

Un cas pràctic seria el següent:

1. Walmart detecta que necessita més unitats d’un producte.
2. El seu sistema envia automàticament una comanda al proveïdor mitjançant un document **EDI 850**.
3. El proveïdor rep la comanda al seu ERP i respon amb un **EDI 855** per confirmar-la.
4. Quan prepara l’enviament, el proveïdor envia un **EDI 856** amb la informació de l’expedició.
5. Finalment, el proveïdor envia la factura amb un **EDI 810**.

Aquest procés evita haver d’enviar correus electrònics o introduir dades manualment. Per això, l’EDI continua sent molt important en empreses de logística, distribució i venda al detall.

### Relació amb ERP

En aquest cas, l’ERP del proveïdor pot estar connectat amb la plataforma de Walmart. Quan arriba una comanda EDI 850, el sistema la pot convertir automàticament en una comanda de venda dins de l’ERP. Després, el mateix ERP pot generar l’avís d’enviament i la factura corresponent.

Això demostra que l’EDI permet que dues empreses intercanviïn dades comercials de manera estructurada, ràpida i automatitzada.


### Exemple de codi JSON d’una comanda de compra

```json
{
  "purchase_order": {
    "order_number": "PO-2026-0045",
    "date": "2026-05-20",
    "customer": {
      "name": "SecureLogistics S.L.",
      "vat": "B12345678",
      "email": "compres@securelogistics.cat"
    },
    "supplier": {
      "name": "Proveïdor Informàtic SA",
      "vat": "A87654321"
    },
    "items": [
      {
        "product_code": "SERV-ERP",
        "description": "Servei d'integració ERP",
        "quantity": 1,
        "unit_price": 850.00
      },
      {
        "product_code": "LIC-CRM",
        "description": "Llicència CRM anual",
        "quantity": 5,
        "unit_price": 120.00
      }
    ],
    "total": 1450.00,
    "currency": "EUR"
  }
}
```

Aquest fragment representa una comanda de compra. Les dades estan organitzades en camps i objectes perquè una altra aplicació les pugui interpretar automàticament.

### Demostració pràctica d’una comanda de compra en JSON

Per demostrar com es pot utilitzar JSON en un entorn ERP, he creat un fitxer anomenat `comanda_compra.json` que representa una comanda de compra. Aquest fitxer conté informació estructurada sobre el número de comanda, la data, el client, el proveïdor, els productes i l’import total.

Primer he creat la carpeta "demo_comanda_json"

<img width="360" height="144" alt="image" src="https://github.com/user-attachments/assets/6b0d7216-fa50-4dbb-8706-96623b08a3b8" />

Dins he creat "comanda_compra.json"

<img width="522" height="740" alt="image" src="https://github.com/user-attachments/assets/4155e63b-0c48-48f7-824a-beea220cb04f" />

Ara he validat el json amb aquesta comanda "python3 -m json.tool comanda_compra.json", com mostra el json ordenat significa que te una estructura valida:

<img width="630" height="761" alt="image" src="https://github.com/user-attachments/assets/43567544-89bb-4a55-a81e-d67b49cd2edf" />

Tot seguit he creat un petit programa que llegeix la comanda 

<img width="673" height="538" alt="image" src="https://github.com/user-attachments/assets/95e92b95-2fde-41fb-869e-0cfb73ba7608" />

Al executar-lo l’aplicació mostra per pantalla les dades de la comanda, com el client, el proveïdor, els productes i el total.

<img width="374" height="514" alt="image" src="https://github.com/user-attachments/assets/50f8a4a6-c924-4e9c-91b0-572333988ee3" />

Aquesta pràctica demostra que JSON permet representar dades empresarials de forma estructurada i que una aplicació externa pot llegir aquestes dades automàticament. En un cas real, un ERP podria enviar una comanda en JSON a una botiga online, a un proveïdor o a una empresa logística mitjançant una API.

---

## 3. Cas pràctic: Estudi d’un ERP — Odoo

He triat **Odoo**, perquè és un ERP molt conegut i té una versió Community de codi obert. A més, és un bon exemple per veure la relació entre ERP, APIs, XML, CSV i mòduls.

<img width="1500" height="1000" alt="image" src="https://github.com/user-attachments/assets/7bc3fa90-6a5c-4a99-a5d1-a9a1cbb86ae1" />

### Importació i exportació de dades en Odoo

Odoo permet **importar i exportar dades** per modificar registres massivament, fer informes o traspassar informació entre sistemes. Disposa d’eines d’importació i exportació de dades dins de l’aplicació, especialment amb fitxers CSV o fulls de càlcul.

Per exemple, es poden importar o exportar:

- clients;
- productes;
- proveïdors;
- comandes;
- factures;
- inventari;
- dades comptables.

El format **CSV** és molt habitual perquè és simple i es pot obrir amb programes com LibreOffice Calc o Excel. Cada línia representa un registre i cada columna representa un camp.

Exemple simple de CSV:

```csv
name,email,phone
Client Exemple,client@example.com,977000000
Empresa Demo,info@empresa-demo.cat,977111111
```

A més, en el desenvolupament d’Odoo també s’utilitzen fitxers **XML** per definir dades, vistes, menús, accions i configuracions. Una de les formes principals de definir dades dins del sistema és mitjançant fitxers XML.

## Cas pràctic: prova d’Odoo en Ubuntu

Per desenvolupar l’apartat dedicat a Odoo, he instal·lat una versió d’Odoo Community en Ubuntu utilitzant Docker. Aquesta opció és adequada perquè permet executar Odoo i PostgreSQL en contenidors separats, sense modificar massa el sistema operatiu principal.

### Instal·lació amb Docker

La idea es instal·lar-lo amb Docker, crear un client/producte i provar importació/exportació CSV. Primer he creat una carpeta per al projecte:

<img width="811" height="138" alt="image" src="https://github.com/user-attachments/assets/891ab9a3-96d9-4a9f-b4e9-a676c5b312e9" />

<img width="389" height="69" alt="image" src="https://github.com/user-attachments/assets/27007d43-a8bd-46ef-b974-02ebb7d3461f" />

<img width="187" height="82" alt="image" src="https://github.com/user-attachments/assets/c1485aa3-b9c5-4632-981e-c3deed681445" />

Despres he creat el .yml 

<img width="467" height="668" alt="image" src="https://github.com/user-attachments/assets/a954c28b-c14d-497c-8c3e-d7c823532234" />

Ara he iniciat el docker

<img width="426" height="267" alt="image" src="https://github.com/user-attachments/assets/9e4b7eb8-a084-4a03-b44a-36e0518ef65b" />

I entrem al localhost desde la web per entrar a odoo, i demana crear una base de dades, he posat les dades seguents:

<img width="947" height="1005" alt="image" src="https://github.com/user-attachments/assets/d78d607b-7393-4897-8f18-f97c3135502d" />

Ara he instalat alguns moduls de prova com CRM, ventas, inventario i facturación

<img width="901" height="407" alt="image" src="https://github.com/user-attachments/assets/26512c59-5aa5-427d-97e9-5f1cef617865" />

<img width="352" height="115" alt="image" src="https://github.com/user-attachments/assets/53954c2b-f234-4da2-be56-a51218f4c7f3" />


<img width="354" height="124" alt="image" src="https://github.com/user-attachments/assets/6154df6a-fab3-4f72-9591-b8033ff29484" />


<img width="376" height="114" alt="image" src="https://github.com/user-attachments/assets/63327c94-7958-4042-a8f8-ef07f9e1b1a9" />

| Mòdul     | Funció                                                |
| --------- | ----------------------------------------------------- |
| CRM       | Gestiona oportunitats comercials i clients potencials |
| Sales     | Gestiona pressupostos i comandes de venda             |
| Inventory | Gestiona productes i estoc                            |
| Invoicing | Gestiona factures                                     |

### Què són els mòduls?

Els **mòduls** d’Odoo són paquets que afegeixen funcionalitats al sistema. Per exemple, hi pot haver un mòdul de vendes, un de comptabilitat, un de CRM, un d’inventari o un de recursos humans.

Un mòdul pot incloure:

- models de dades;
- pantalles o vistes;
- menús;
- informes;
- permisos;
- dades de configuració;
- automatitzacions.

És important que els llenguatges de marques siguin estandarditzats perquè permeten que diferents mòduls i sistemes puguin entendre la mateixa estructura de dades. Per exemple, si una vista d’Odoo es defineix amb XML, el sistema sap interpretar com s’han de mostrar els camps, els formularis o els menús.

Les vistes d’Odoo es defineixen en fitxers XML, cosa que facilita modificar la interfície sense haver de canviar directament la lògica interna del programa.

### Què és FacturaE?

**FacturaE** és el format oficial de factura electrònica utilitzat a Espanya. Està basat en **XML**, és a dir, la factura no és només un PDF visual, sinó un fitxer estructurat amb etiquetes que indiquen les dades de l’emissor, el receptor, els imports, els impostos i les línies de factura.

La seva relació amb XML és directa: FacturaE utilitza una estructura XML perquè les factures puguin ser llegides automàticament per programes de facturació, administracions públiques i plataformes com FACe. En la facturació amb administracions públiques a Espanya, FacturaE continua sent un format clau per enviar factures electròniques.

### Exemple simplificat d’estructura XML de factura

```xml
<Facturae>
  <FileHeader>
    <SchemaVersion>3.2.2</SchemaVersion>
    <Modality>I</Modality>
    <InvoiceIssuerType>EM</InvoiceIssuerType>
  </FileHeader>

  <Parties>
    <SellerParty>
      <TaxIdentification>
        <TaxIdentificationNumber>B12345678</TaxIdentificationNumber>
      </TaxIdentification>
    </SellerParty>

    <BuyerParty>
      <TaxIdentification>
        <TaxIdentificationNumber>A87654321</TaxIdentificationNumber>
      </TaxIdentification>
    </BuyerParty>
  </Parties>

  <Invoices>
    <Invoice>
      <InvoiceHeader>
        <InvoiceNumber>F2026-001</InvoiceNumber>
      </InvoiceHeader>
      <InvoiceIssueData>
        <IssueDate>2026-05-20</IssueDate>
      </InvoiceIssueData>
      <TaxesOutputs>
        <Tax>
          <TaxTypeCode>01</TaxTypeCode>
          <TaxRate>21.00</TaxRate>
        </Tax>
      </TaxesOutputs>
    </Invoice>
  </Invoices>
</Facturae>
```

Aquest exemple mostra que XML utilitza etiquetes per identificar cada part de la factura.

---

## 4. Conclusions i reflexió

Un administrador de sistemes ASIX ha de conèixer els llenguatges de marques perquè avui dia els sistemes empresarials estan connectats constantment amb altres plataformes. Un ERP o un CRM no treballa de manera aïllada: pot enviar factures, rebre comandes d’una botiga online, comunicar-se amb bancs, exportar dades a fulls de càlcul o integrar-se amb empreses de transport.

Formats com **XML, JSON, CSV o EDI** permeten que les dades “viatgin” entre sistemes diferents. Per això, un tècnic d’ASIX ha de saber interpretar aquests formats, detectar errors d’importació, configurar integracions, revisar fitxers i entendre com es comuniquen les aplicacions.

En resum, conèixer llenguatges de marques no és només saber escriure etiquetes XML o claus JSON, sinó entendre com es mou la informació dins d’una empresa real. Aquesta competència és molt important per mantenir sistemes ERP/CRM, automatitzar processos i evitar errors en dades crítiques com clients, factures, comandes o inventari.

Personalment, crec que aquesta activitat m’ha ajudat a entendre que els llenguatges de marques no són només teoria, sinó una part molt important del funcionament real de les empreses. Quan un ERP importa productes amb CSV, envia factures en XML o rep comandes en JSON, està utilitzant estructures de dades que un administrador de sistemes ha de saber interpretar i mantenir. Per això, en el perfil d’ASIX, aquests coneixements són útils tant per resoldre errors com per configurar integracions entre plataformes.

---

## Fonts consultades

- Documentació oficial d’Odoo sobre importació i exportació de dades: <https://www.odoo.com/documentation/19.0/applications/essentials/export_import_data.html>
- Documentació oficial d’Odoo per a desenvolupadors: <https://www.odoo.com/documentation/19.0/developer/reference/backend/data.html>
- Documentació oficial d’Odoo sobre mòduls i desenvolupament backend: <https://www.odoo.com/documentation/19.0/developer/tutorials/backend.html>
- Documentació oficial d’Odoo sobre vistes XML: <https://www.odoo.com/documentation/19.0/developer/tutorials/server_framework_101/06_basicviews.html>
- Informació sobre FacturaE: <https://www.facturae.gob.es>
- Informació sobre estàndards EDI: <https://www.gs1.org/standards/edi>
- Documentació oficial de Walmart Developers sobre la interfície EDI per a proveïdors: <https://developer.walmart.com/suppliers/docs/electronic-data-exchange-edi-interface>
- Guia oficial de Walmart sobre el document EDI 850 Purchase Order: <https://developer.walmart.com/suppliers/docs/850-purchase-order>
