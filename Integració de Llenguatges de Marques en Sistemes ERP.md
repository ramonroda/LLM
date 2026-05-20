# Tasca de Recerca: Integració de Llenguatges de Marques en Sistemes ERP/CRM

## 1. Fonaments de Sistemes Empresarials

### Què és un ERP?

Un **ERP** (*Enterprise Resource Planning*) és un sistema de gestió empresarial que integra diferents àrees d’una empresa en una mateixa plataforma: comptabilitat, compres, vendes, magatzem, recursos humans, producció, facturació, etc.

La seva funció principal és centralitzar la informació perquè tots els departaments treballin amb les mateixes dades i evitar duplicitats o errors.

### Què és un CRM?

Un **CRM** (*Customer Relationship Management*) és un sistema orientat a gestionar la relació amb els clients. Serveix per controlar contactes, oportunitats de venda, seguiment comercial, incidències, campanyes de màrqueting i atenció al client.

Mentre que un ERP gestiona l’activitat interna de l’empresa, un CRM se centra sobretot en la relació amb els clients.

---

## Exemples d’ERP

| Tipus | Exemples |
|---|---|
| Programari lliure / Open Source | Odoo Community, ERPNext, Dolibarr |
| Propietari | SAP ERP / SAP S/4HANA, Microsoft Dynamics 365, Oracle NetSuite |

## Exemples de CRM

| Tipus | Exemples |
|---|---|
| Programari lliure / Open Source | SuiteCRM, Odoo CRM Community, EspoCRM |
| Propietari | Salesforce, HubSpot CRM, Microsoft Dynamics 365 Sales |

---

## Instal·lació On-premise i SaaS

Una instal·lació **On-premise** significa que el programari s’instal·la en servidors propis de l’empresa. L’empresa és responsable del manteniment, les còpies de seguretat, la seguretat, les actualitzacions i la infraestructura.

En canvi, una solució **SaaS** (*Software as a Service*) o **Cloud** funciona al núvol. L’empresa accedeix al sistema mitjançant Internet i normalment paga una subscripció. El proveïdor s’encarrega dels servidors, les actualitzacions i part de la seguretat.

Alguns exemples de sistemes que poden funcionar en modalitat SaaS són Odoo Online, Salesforce o Microsoft Dynamics 365.

---

# 2. El paper de l’XML i JSON en l’intercanvi de dades

## Web Services i APIs

Els **Web Services** o **APIs** són mecanismes que permeten que dues aplicacions diferents es comuniquin entre elles.

Per exemple, un ERP pot:

- enviar dades de facturació a una gestoria;
- rebre comandes d’una botiga online;
- consultar l’estat d’un enviament amb una empresa logística;
- connectar-se amb un banc;
- enviar una factura electrònica a una administració pública.

Els formats **JSON** i **XML** s’utilitzen per estructurar aquestes dades de manera que siguin llegibles per diferents sistemes.

## Ús de JSON i XML en un ERP

Una botiga online pot enviar una comanda a l’ERP en format JSON. L’ERP rep la informació del client, els productes, les quantitats i l’import total, i automàticament pot crear una comanda de venda.

També pot passar a l’inrevés: l’ERP pot exportar una factura en XML perquè una administració pública o una altra plataforma la pugui llegir.

**JSON** és molt habitual en APIs modernes perquè és més lleuger i fàcil de treballar amb aplicacions web.

**XML**, en canvi, continua sent molt important en entorns més formals o regulats, com la facturació electrònica, alguns serveis bancaris o intercanvis amb administracions públiques.

---

## Què és EDI?

L’**EDI** (*Electronic Data Interchange*) és l’intercanvi electrònic de documents comercials entre empreses seguint formats estandarditzats.

Pot servir per enviar:

- comandes;
- albarans;
- factures;
- avisos d’expedició;
- confirmacions de recepció.

L’objectiu és evitar haver d’introduir les dades manualment i reduir errors.

L’EDI encara té molta rellevància en el sector logístic i en la cadena de subministrament, perquè permet automatitzar la comunicació entre fabricants, proveïdors, magatzems, distribuïdors i clients.

---

## Exemple de codi JSON d’una comanda de compra

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
} ```
s

