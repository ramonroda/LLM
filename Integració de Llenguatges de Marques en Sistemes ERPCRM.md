# Tasca de Recerca: Integració de Llenguatges de Marques en Sistemes ERP/CRM

## 1. Fonaments de Sistemes Empresarials

### Què és un ERP?

Un **ERP** (*Enterprise Resource Planning*) és un sistema de gestió empresarial que integra diferents àrees d’una empresa en una mateixa plataforma: comptabilitat, compres, vendes, magatzem, recursos humans, producció, facturació, etc. La seva funció principal és centralitzar la informació perquè tots els departaments treballin amb les mateixes dades.

### Què és un CRM?

Un **CRM** (*Customer Relationship Management*) és un sistema orientat a gestionar la relació amb els clients. Serveix per controlar contactes, oportunitats de venda, seguiment comercial, incidències, campanyes de màrqueting i atenció al client.

### Exemples d’ERP

| Tipus | Exemples |
|---|---|
| Programari lliure / Open Source | Odoo Community, ERPNext, Dolibarr |
| Propietari | SAP ERP / SAP S/4HANA, Microsoft Dynamics 365, Oracle NetSuite |

### Exemples de CRM

| Tipus | Exemples |
|---|---|
| Programari lliure / Open Source | SuiteCRM, Odoo CRM Community, EspoCRM |
| Propietari | Salesforce, HubSpot CRM, Microsoft Dynamics 365 Sales |

### Instal·lació On-premise i SaaS

Una instal·lació **On-premise** significa que el programari s’instal·la en servidors propis de l’empresa. L’empresa és responsable del manteniment, les còpies de seguretat, la seguretat, les actualitzacions i la infraestructura.

En canvi, una solució **SaaS o Cloud** funciona al núvol. L’empresa accedeix al sistema mitjançant Internet i normalment paga una subscripció. El proveïdor s’encarrega dels servidors, les actualitzacions i part de la seguretat. Per exemple, moltes empreses utilitzen Odoo, Salesforce o Microsoft Dynamics 365 en modalitat SaaS.

---

## 2. El paper de l’XML i JSON en l’intercanvi de dades

### Web Services i APIs

Els **Web Services** o **APIs** són mecanismes que permeten que dues aplicacions diferents es comuniquin entre elles. Per exemple, un ERP pot enviar dades de facturació a una gestoria, rebre comandes d’una botiga online o consultar l’estat d’un enviament amb una empresa logística.

Els formats **JSON** i **XML** s’utilitzen per estructurar aquestes dades de manera que siguin llegibles per diferents sistemes.

Per exemple, una botiga online pot enviar una comanda a l’ERP en format JSON. L’ERP rep la informació del client, els productes, les quantitats i l’import total, i automàticament pot crear una comanda de venda. També pot passar a l’inrevés: l’ERP pot exportar una factura en XML perquè una administració pública o una altra plataforma la pugui llegir.

JSON és molt habitual en APIs modernes perquè és més lleuger i fàcil de treballar amb aplicacions web. XML, en canvi, continua sent molt important en entorns més formals o regulats, com la facturació electrònica, alguns serveis bancaris o intercanvis amb administracions públiques.

### Què és EDI?

L’**EDI** (*Electronic Data Interchange*) és l’intercanvi electrònic de documents comercials entre empreses seguint formats estandarditzats. Pot servir per enviar comandes, albarans, factures, avisos d’expedició o confirmacions de recepció sense haver d’introduir les dades manualment.

Encara té molta rellevància en el sector logístic i en la cadena de subministrament, perquè permet automatitzar la comunicació entre fabricants, proveïdors, magatzems, distribuïdors i clients. Encara avui moltes empreses utilitzen estàndards EDI per automatitzar transaccions comercials entre sistemes.

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

---

## 3. Cas pràctic: Estudi d’un ERP — Odoo

He triat **Odoo**, perquè és un ERP molt conegut i té una versió Community de codi obert. A més, és un bon exemple per veure la relació entre ERP, APIs, XML, CSV i mòduls.

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

---

## Fonts consultades

- Documentació oficial d’Odoo sobre importació i exportació de dades: <https://www.odoo.com/documentation/19.0/applications/essentials/export_import_data.html>
- Documentació oficial d’Odoo per a desenvolupadors: <https://www.odoo.com/documentation/19.0/developer/reference/backend/data.html>
- Documentació oficial d’Odoo sobre mòduls i desenvolupament backend: <https://www.odoo.com/documentation/19.0/developer/tutorials/backend.html>
- Documentació oficial d’Odoo sobre vistes XML: <https://www.odoo.com/documentation/19.0/developer/tutorials/server_framework_101/06_basicviews.html>
- Informació sobre FacturaE: <https://www.facturae.gob.es>
- Informació sobre estàndards EDI: <https://www.gs1.org/standards/edi>
