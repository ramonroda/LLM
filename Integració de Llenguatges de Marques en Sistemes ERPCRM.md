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

- Tot Seguit he creat 1 clients i 2 productes ficticis per fer les proves

<img width="588" height="783" alt="image" src="https://github.com/user-attachments/assets/5b3e19f3-6ecc-4d92-82b5-c182e3ba0b07" />

<img width="398" height="277" alt="image" src="https://github.com/user-attachments/assets/86194514-2598-4b92-aa56-599ffd95a9ab" />

- Productes

<img width="530" height="407" alt="image" src="https://github.com/user-attachments/assets/e46f13f8-a587-48a4-ac0a-1702f99ada9f" />

<img width="434" height="314" alt="image" src="https://github.com/user-attachments/assets/077629ae-919a-4c81-9481-e4ee6a101def" />

<img width="752" height="207" alt="image" src="https://github.com/user-attachments/assets/b2a1c68e-c895-4045-919e-e22dd7eb4d06" />

--

- Ara vaig a fer la prova de exportar dades en CSV

<img width="322" height="298" alt="image" src="https://github.com/user-attachments/assets/99d96a7d-365c-4b88-ac54-e7f0bd648603" />

Exportare alguns camps com aquests

<img width="660" height="294" alt="image" src="https://github.com/user-attachments/assets/c3595f15-900a-474a-8e81-031f04f05c4c" />

Despres d'exportar, veiem que conte els camps correctes

<img width="593" height="124" alt="image" src="https://github.com/user-attachments/assets/a77c4d74-0642-4d5f-a516-ebf8baed9003" />

Això demostra que Odoo pot treure dades en un format que després pot llegir una altra aplicació.

- Prova de importacio de dades a Odoo, primer he creat un csv i he posat les seguents dades

<img width="524" height="153" alt="image" src="https://github.com/user-attachments/assets/859f7506-04f6-4501-aa45-f7a0aa8de691" />

<img width="350" height="130" alt="image" src="https://github.com/user-attachments/assets/c49b3c1b-4226-4a07-b30e-c92cb53dc3bd" />

Veiem que s'han exportat correctament

<img width="1112" height="328" alt="image" src="https://github.com/user-attachments/assets/d536227f-c0d2-43d0-bc09-8384a99e27dd" />

Odoo pot importar dades externes en CSV i convertir-les en registres interns del sistema ERP.

### Ús d’XML en Odoo

A més del format CSV per importar i exportar dades, Odoo també utilitza el llenguatge **XML** en el desenvolupament dels seus mòduls. XML és molt important perquè permet definir l’estructura de diferents elements del sistema, com ara vistes, menús, accions, permisos o dades de configuració.

En Odoo, un fitxer XML pot servir per indicar com s’ha de mostrar una pantalla dins de l’ERP. Per exemple, es pot definir quins camps apareixen en el formulari d’un client, quins botons hi ha disponibles o com s’organitzen els menús.

Això demostra que XML no només s’utilitza per intercanviar dades entre aplicacions, sinó també per configurar i ampliar sistemes empresarials com un ERP.

#### Exemple simplificat d’una vista XML en Odoo

```xml
<odoo>
    <record id="view_partner_form_custom" model="ir.ui.view">
        <field name="name">res.partner.form.custom</field>
        <field name="model">res.partner</field>
        <field name="arch" type="xml">
            <form string="Contacte">
                <sheet>
                    <group>
                        <field name="name"/>
                        <field name="email"/>
                        <field name="phone"/>
                    </group>
                </sheet>
            </form>
        </field>
    </record>
</odoo>
```
#### Explicació del codi XML

Aquest fragment XML representa una vista de formulari dins d’Odoo. Encara que és un exemple simplificat, ajuda a entendre com Odoo utilitza XML per definir parts de la seva interfície.

En aquest cas, la vista està relacionada amb el model `res.partner`, que en Odoo s’utilitza per gestionar contactes, clients i proveïdors. El codi indica que el formulari ha de mostrar tres camps principals: el nom, el correu electrònic i el telèfon.

| Element XML | Funció |
|---|---|
| `<odoo>` | És l’etiqueta principal del fitxer XML d’Odoo. Tot el contingut del fitxer queda dins d’aquesta etiqueta. |
| `<record>` | Defineix un registre nou dins del sistema. En aquest cas, el registre correspon a una vista. |
| `id="view_partner_form_custom"` | És l’identificador intern d’aquesta vista. Serveix perquè Odoo la pugui reconèixer. |
| `model="ir.ui.view"` | Indica que el registre que s’està creant és una vista de la interfície d’Odoo. |
| `<field name="name">` | Dona un nom tècnic a la vista. |
| `<field name="model">res.partner</field>` | Indica que aquesta vista pertany al model de contactes, clients o proveïdors. |
| `<field name="arch" type="xml">` | Conté l’estructura XML de la vista. |
| `<form string="Contacte">` | Defineix que la vista serà un formulari amb el títol “Contacte”. |
| `<sheet>` | Representa la zona principal del formulari. |
| `<group>` | Agrupa diferents camps dins del formulari perquè es mostrin de manera ordenada. |
| `<field name="name"/>` | Mostra el camp del nom del contacte. |
| `<field name="email"/>` | Mostra el camp del correu electrònic. |
| `<field name="phone"/>` | Mostra el camp del telèfon. |

### Per què és important XML en Odoo?

XML és important en Odoo perquè permet modificar i ampliar el sistema d’una manera estructurada. Gràcies a XML, un desenvolupador pot crear o modificar pantalles, afegir menús, definir accions o carregar dades inicials dins del sistema.

Per exemple, si una empresa necessita que el formulari dels clients mostri uns camps concrets, es pot crear o modificar una vista XML. Això fa que Odoo sigui un ERP flexible i adaptable a les necessitats de cada empresa.

A més, XML permet separar la part visual o estructural de la lògica del programa. És a dir, la lògica principal pot estar programada en Python, mentre que les vistes, menús i accions poden estar definides en fitxers XML.

### Relació amb els mòduls d’Odoo

Els mòduls d’Odoo són paquets que afegeixen funcionalitats al sistema. Per exemple, hi pot haver un mòdul de vendes, un de CRM, un d’inventari o un de facturació.

Un mòdul d’Odoo pot incloure diferents tipus de fitxers:

| Tipus de fitxer | Funció dins d’Odoo |
|---|---|
| Python | Defineix la lògica del mòdul i els models de dades. |
| XML | Defineix vistes, formularis, menús, accions i dades de configuració. |
| CSV | Serveix per carregar dades simples, com permisos o registres inicials. |
| Fitxers de seguretat | Controlen quins usuaris poden accedir a cada part del sistema. |

Per aquest motiu, el llenguatge XML és una peça clau en el desenvolupament de mòduls. Permet que Odoo entengui com s’han de mostrar les dades i com s’ha d’organitzar la interfície.

### Importància dels llenguatges de marques en Odoo

L’ús d’XML i CSV en Odoo demostra que els llenguatges de marques i els formats estructurats són essencials dins d’un ERP.

El format **CSV** és útil per importar i exportar dades tabulars, com clients, productes o contactes. En canvi, el format **XML** és més adequat per definir estructures més complexes, com vistes, formularis, menús, accions o configuracions internes.

| Format | Ús principal en Odoo | Exemple d’ús |
|---|---|---|
| CSV | Importació i exportació de dades simples | Llista de clients, productes o proveïdors |
| XML | Definició d’estructures internes del sistema | Formularis, vistes, menús i accions |
| JSON | Comunicació amb aplicacions externes mitjançant APIs | Enviament de dades a una botiga online o una app externa |

Això és important perquè un administrador de sistemes o un tècnic d’ASIX pot necessitar revisar aquests fitxers per detectar errors, configurar importacions de dades o entendre com s’ha instal·lat un mòdul dins de l’ERP.

### Exemple pràctic relacionat amb Odoo

Un exemple realista seria una empresa que necessita importar una llista de clients a Odoo. Aquesta empresa podria preparar un fitxer CSV amb les dades dels clients i importar-lo directament dins del sistema.

Exemple de fitxer CSV:

```csv
name,email,phone
Client Prova 1,client1@example.com,977000001
Client Prova 2,client2@example.com,977000002
Client Prova 3,client3@example.com,977000003
```

Després d’importar aquest fitxer, Odoo crea automàticament els contactes dins del mòdul corresponent. Això evita haver d’introduir les dades manualment una per una.

D’altra banda, si es vol modificar la forma com es mostra el formulari d’un client, es podria utilitzar XML per definir o adaptar aquesta vista.

### Conclusió del cas pràctic d’Odoo

Aquesta prova amb Odoo permet veure que un ERP no només serveix per gestionar informació empresarial, sinó que també necessita formats estructurats per importar, exportar i configurar dades.

D’una banda, el CSV facilita el moviment de dades entre Odoo i altres aplicacions, com fulls de càlcul, altres ERP o scripts d’automatització. D’altra banda, XML permet definir parts internes del sistema, com les vistes, formularis i menús dels mòduls.

Per tant, conèixer llenguatges de marques com XML i formats com CSV o JSON és molt útil per administrar i mantenir un sistema ERP. Aquests coneixements permeten entendre millor com es mouen les dades dins d’una empresa i com es poden integrar diferents aplicacions entre elles.

### Què són els mòduls?

Els **mòduls** d’Odoo són paquets que afegeixen funcionalitats al sistema. Per exemple, hi pot haver un mòdul de vendes, un de comptabilitat, un de CRM, un d’inventari o un de recursos humans.

<img width="697" height="590" alt="image" src="https://github.com/user-attachments/assets/91f3a223-09e2-4597-8fde-f6b7b99058c6" />

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

## Què és FacturaE?

**FacturaE** és el format de factura electrònica utilitzat a Espanya. Es basa en el llenguatge **XML**, cosa que permet representar les dades d’una factura de manera estructurada i llegible per programes informàtics.

Una factura en format FacturaE no és simplement un PDF amb una factura visual, sinó un fitxer electrònic que conté etiquetes XML amb informació com:

- dades de l’emissor;
- dades del receptor;
- número de factura;
- data d’emissió;
- base imposable;
- impostos;
- import total;
- línies de productes o serveis.

A Espanya, les factures electròniques enviades a les administracions públiques han de seguir el format estructurat **FacturaE 3.2.x** i incloure signatura electrònica XAdES. Aquesta obligació es va establir amb la Llei 25/2013 per impulsar la factura electrònica en el sector públic.  
Font: Portal oficial FacturaE: https://www.facturae.gob.es/formato

### Relació entre FacturaE i XML

FacturaE està directament relacionat amb XML perquè utilitza aquest llenguatge per organitzar la informació de la factura.

Per exemple, una factura pot contenir etiquetes com:

```xml
<InvoiceNumber>F2026-001</InvoiceNumber>
<IssueDate>2026-05-20</IssueDate>
<TaxRate>21.00</TaxRate>
<TotalGrossAmount>1450.00</TotalGrossAmount>
```

Aquestes etiquetes indiquen clarament quin és el número de factura, la data, el percentatge d’IVA i l’import total.

Això permet que diferents sistemes, com un ERP, una administració pública o una plataforma de facturació, puguin llegir automàticament la factura sense haver d’introduir les dades manualment.

### Exemple simplificat de FacturaE en XML

A continuació es mostra un exemple molt simplificat d’una factura electrònica inspirada en el format FacturaE:

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
            <LegalEntity>
                <CorporateName>SecureLogistics S.L.</CorporateName>
            </LegalEntity>
        </SellerParty>

        <BuyerParty>
            <TaxIdentification>
                <TaxIdentificationNumber>A87654321</TaxIdentificationNumber>
            </TaxIdentification>
            <LegalEntity>
                <CorporateName>Ajuntament de Roquetes</CorporateName>
            </LegalEntity>
        </BuyerParty>
    </Parties>

    <Invoices>
        <Invoice>
            <InvoiceHeader>
                <InvoiceNumber>F2026-001</InvoiceNumber>
                <InvoiceSeriesCode>A</InvoiceSeriesCode>
            </InvoiceHeader>

            <InvoiceIssueData>
                <IssueDate>2026-05-20</IssueDate>
            </InvoiceIssueData>

            <Items>
                <InvoiceLine>
                    <ItemDescription>Servei d'integració ERP</ItemDescription>
                    <Quantity>1</Quantity>
                    <UnitPriceWithoutTax>850.00</UnitPriceWithoutTax>
                    <TotalCost>850.00</TotalCost>
                </InvoiceLine>

                <InvoiceLine>
                    <ItemDescription>Llicència CRM anual</ItemDescription>
                    <Quantity>5</Quantity>
                    <UnitPriceWithoutTax>120.00</UnitPriceWithoutTax>
                    <TotalCost>600.00</TotalCost>
                </InvoiceLine>
            </Items>

            <InvoiceTotals>
                <TotalGrossAmount>1450.00</TotalGrossAmount>
                <TotalTaxOutputs>304.50</TotalTaxOutputs>
                <InvoiceTotal>1754.50</InvoiceTotal>
            </InvoiceTotals>
        </Invoice>
    </Invoices>
</Facturae>
```

### Explicació del codi XML

| Element XML | Funció |
|---|---|
| `<Facturae>` | Etiqueta principal del document. |
| `<FileHeader>` | Conté informació general del fitxer FacturaE. |
| `<SchemaVersion>` | Indica la versió del format utilitzat, per exemple 3.2.2. |
| `<Parties>` | Agrupa les dades de les parts que intervenen en la factura. |
| `<SellerParty>` | Representa l’empresa o persona que emet la factura. |
| `<BuyerParty>` | Representa el client o entitat que rep la factura. |
| `<TaxIdentificationNumber>` | Conté el NIF o CIF de l’emissor o receptor. |
| `<Invoices>` | Agrupa les factures incloses en el fitxer. |
| `<InvoiceNumber>` | Número de factura. |
| `<IssueDate>` | Data d’emissió de la factura. |
| `<Items>` | Conté les línies de productes o serveis facturats. |
| `<InvoiceLine>` | Representa una línia concreta de la factura. |
| `<InvoiceTotals>` | Agrupa els imports totals de la factura. |
| `<InvoiceTotal>` | Import final de la factura. |

### Demostració pràctica en Ubuntu

Per demostrar que FacturaE està basat en XML i que les seves dades poden ser llegides per una aplicació, es pot crear un fitxer XML i llegir-lo amb Python.

Primer, creo un fitxer anomenat `facturae_exemple.xml`:

```bash
nano facturae_exemple.xml
```

Hi afegeixo el contingut XML anterior i guardo el fitxer.

Després, creo un programa Python per llegir algunes dades de la factura:

```bash
nano llegir_facturae.py
```

Codi del programa:

```python
import xml.etree.ElementTree as ET

arbre = ET.parse("facturae_exemple.xml")
arrel = arbre.getroot()

numero_factura = arrel.find(".//InvoiceNumber").text
data_factura = arrel.find(".//IssueDate").text
emissor = arrel.find(".//SellerParty/LegalEntity/CorporateName").text
receptor = arrel.find(".//BuyerParty/LegalEntity/CorporateName").text
total = arrel.find(".//InvoiceTotal").text

print("=== FACTURA ELECTRÒNICA FACTURAE ===")
print("Número de factura:", numero_factura)
print("Data:", data_factura)
print("Emissor:", emissor)
print("Receptor:", receptor)
print("Total factura:", total, "€")

print("\nLínies de factura:")
for linia in arrel.findall(".//InvoiceLine"):
    descripcio = linia.find("ItemDescription").text
    quantitat = linia.find("Quantity").text
    preu = linia.find("UnitPriceWithoutTax").text
    subtotal = linia.find("TotalCost").text

    print("-", descripcio)
    print("  Quantitat:", quantitat)
    print("  Preu unitari sense IVA:", preu, "€")
    print("  Subtotal:", subtotal, "€")
```

Executo el programa:

```bash
python3 llegir_facturae.py
```

<img width="417" height="411" alt="image" src="https://github.com/user-attachments/assets/945a2563-10da-4c0f-b0f9-4e10265a0e3f" />


### Relació amb ERP

En un cas real, un ERP com Odoo, SAP o Microsoft Dynamics podria generar una factura amb les dades del client, els productes i els imports. Després, aquesta factura es podria exportar en format FacturaE per enviar-la a una administració pública o a una plataforma de facturació electrònica.

Això demostra que XML és útil perquè permet que les dades d’una factura siguin llegides automàticament per diferents sistemes.


FacturaE és un bon exemple de l’ús real de XML en l’àmbit empresarial i administratiu. Gràcies a aquest format, una factura electrònica pot ser processada automàticament per un ERP, una plataforma pública o un sistema de comptabilitat.

Per aquest motiu, un administrador de sistemes ha de conèixer XML i entendre com s’estructuren aquests documents, ja que pot haver de configurar sistemes de facturació, revisar errors d’importació o comprovar que una factura electrònica compleix l’estructura correcta.

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
