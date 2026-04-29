---
description: Represents a sales order entity in Dynamics 365 Business Central. Sales orders are documents used to record the sale of goods or services to customers. They include header information (customer, dates, payment terms) and line items specifying the products or services being sold.
layout: schema
name: Sales Order
properties_list:
- description: ETag for optimistic concurrency control
  name: '@odata.etag'
  type: string
- description: The unique identifier (GUID) of the sales order
  name: id
  type: string
- description: The sales order number assigned from a number series
  name: number
  type: string
- description: An external reference number (e.g., a customer PO number)
  name: externalDocumentNumber
  type: string
- description: The date when the sales order was created
  name: orderDate
  type: string
- description: The date used for posting the sales order to the general ledger
  name: postingDate
  type: string
- description: The unique identifier of the sell-to customer
  name: customerId
  type: string
- description: The customer number of the sell-to customer
  name: customerNumber
  type: string
- description: The name of the sell-to customer
  name: customerName
  type: string
- description: The name of the bill-to party
  name: billToName
  type: string
- description: The unique identifier of the bill-to customer
  name: billToCustomerId
  type: string
- description: The customer number of the bill-to customer
  name: billToCustomerNumber
  type: string
- description: The name for the ship-to address
  name: shipToName
  type: string
- description: The contact person at the ship-to address
  name: shipToContact
  type: string
- description: First line of the sell-to address
  name: sellToAddressLine1
  type: string
- description: Second line of the sell-to address
  name: sellToAddressLine2
  type: string
- description: The city of the sell-to address
  name: sellToCity
  type: string
- description: The country/region code of the sell-to address
  name: sellToCountry
  type: string
- description: The state or province code of the sell-to address
  name: sellToState
  type: string
- description: The postal code of the sell-to address
  name: sellToPostCode
  type: string
- description: The unique identifier of the currency
  name: currencyId
  type: string
- description: The currency code (e.g., USD, EUR) for the sales order
  name: currencyCode
  type: string
- description: Indicates whether the prices on the order include tax
  name: pricesIncludeTax
  type: boolean
- description: The unique identifier of the payment terms
  name: paymentTermsId
  type: string
- description: The unique identifier of the shipment method
  name: shipmentMethodId
  type: string
- description: The salesperson code assigned to the order
  name: salesperson
  type: string
- description: The date the customer has requested delivery
  name: requestedDeliveryDate
  type: string
- description: The total invoice discount amount applied to the order
  name: discountAmount
  type: number
- description: Indicates whether discounts are applied before tax calculation
  name: discountAppliedBeforeTax
  type: boolean
- description: The total amount of the order excluding tax (read-only)
  name: totalAmountExcludingTax
  type: number
- description: The total tax amount on the order (read-only)
  name: totalTaxAmount
  type: number
- description: The total amount of the order including tax (read-only)
  name: totalAmountIncludingTax
  type: number
- description: Indicates whether all lines on the order have been fully shipped (read-only)
  name: fullyShipped
  type: boolean
- description: The current status of the sales order (read-only)
  name: status
  type: string
- description: The date and time the sales order was last modified (read-only)
  name: lastModifiedDateTime
  type: string
- description: The phone number associated with the order
  name: phoneNumber
  type: string
- description: The email address associated with the order
  name: email
  type: string
- description: The line items on the sales order
  name: salesOrderLines
  type: array
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/sales-order.json
slug: sales-order
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://example.com/schemas/navision/sales-order.json\",\n  \"title\": \"Sales Order\",\n  \"description\": \"Represents a sales order entity in Dynamics 365 Business Central. Sales orders are documents used to record the sale of goods or services to customers. They include header information (customer, dates, payment terms) and line items specifying the products or services being sold.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"@odata.etag\": {\n      \"type\": \"string\",\n      \"description\": \"ETag for optimistic concurrency control\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier (GUID) of the sales order\"\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"maxLength\": 20,\n      \"description\": \"The sales order number assigned from a number series\"\n    },\n    \"externalDocumentNumber\"\
  : {\n      \"type\": \"string\",\n      \"maxLength\": 35,\n      \"description\": \"An external reference number (e.g., a customer PO number)\"\n    },\n    \"orderDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The date when the sales order was created\"\n    },\n    \"postingDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The date used for posting the sales order to the general ledger\"\n    },\n    \"customerId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the sell-to customer\"\n    },\n    \"customerNumber\": {\n      \"type\": \"string\",\n      \"maxLength\": 20,\n      \"description\": \"The customer number of the sell-to customer\"\n    },\n    \"customerName\": {\n      \"type\": \"string\",\n      \"maxLength\": 100,\n      \"description\": \"The name of the sell-to customer\"\n    },\n    \"billToName\": {\n      \"\
  type\": \"string\",\n      \"maxLength\": 100,\n      \"description\": \"The name of the bill-to party\"\n    },\n    \"billToCustomerId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the bill-to customer\"\n    },\n    \"billToCustomerNumber\": {\n      \"type\": \"string\",\n      \"maxLength\": 20,\n      \"description\": \"The customer number of the bill-to customer\"\n    },\n    \"shipToName\": {\n      \"type\": \"string\",\n      \"maxLength\": 100,\n      \"description\": \"The name for the ship-to address\"\n    },\n    \"shipToContact\": {\n      \"type\": \"string\",\n      \"maxLength\": 100,\n      \"description\": \"The contact person at the ship-to address\"\n    },\n    \"sellToAddressLine1\": {\n      \"type\": \"string\",\n      \"maxLength\": 100,\n      \"description\": \"First line of the sell-to address\"\n    },\n    \"sellToAddressLine2\": {\n      \"type\": \"string\",\n      \"maxLength\": 50,\n\
  \      \"description\": \"Second line of the sell-to address\"\n    },\n    \"sellToCity\": {\n      \"type\": \"string\",\n      \"maxLength\": 30,\n      \"description\": \"The city of the sell-to address\"\n    },\n    \"sellToCountry\": {\n      \"type\": \"string\",\n      \"maxLength\": 10,\n      \"description\": \"The country/region code of the sell-to address\"\n    },\n    \"sellToState\": {\n      \"type\": \"string\",\n      \"maxLength\": 20,\n      \"description\": \"The state or province code of the sell-to address\"\n    },\n    \"sellToPostCode\": {\n      \"type\": \"string\",\n      \"maxLength\": 20,\n      \"description\": \"The postal code of the sell-to address\"\n    },\n    \"currencyId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the currency\"\n    },\n    \"currencyCode\": {\n      \"type\": \"string\",\n      \"maxLength\": 10,\n      \"description\": \"The currency code (e.g., USD, EUR) for\
  \ the sales order\"\n    },\n    \"pricesIncludeTax\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the prices on the order include tax\"\n    },\n    \"paymentTermsId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the payment terms\"\n    },\n    \"shipmentMethodId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the shipment method\"\n    },\n    \"salesperson\": {\n      \"type\": \"string\",\n      \"maxLength\": 20,\n      \"description\": \"The salesperson code assigned to the order\"\n    },\n    \"requestedDeliveryDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The date the customer has requested delivery\"\n    },\n    \"discountAmount\": {\n      \"type\": \"number\",\n      \"description\": \"The total invoice discount amount applied to the order\"\n    },\n    \"discountAppliedBeforeTax\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether discounts are applied before tax calculation\"\n    },\n    \"totalAmountExcludingTax\": {\n      \"type\": \"number\",\n      \"description\": \"The total amount of the order excluding tax (read-only)\",\n      \"readOnly\": true\n    },\n    \"totalTaxAmount\": {\n      \"type\": \"number\",\n      \"description\": \"The total tax amount on the order (read-only)\",\n      \"readOnly\": true\n    },\n    \"totalAmountIncludingTax\": {\n      \"type\": \"number\",\n      \"description\": \"The total amount of the order including tax (read-only)\",\n      \"readOnly\": true\n    },\n    \"fullyShipped\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether all lines on the order have been fully shipped (read-only)\",\n      \"readOnly\": true\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"Draft\", \"In Review\", \"Open\", \"Released\"],\n      \"description\"\
  : \"The current status of the sales order (read-only)\",\n      \"readOnly\": true\n    },\n    \"lastModifiedDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the sales order was last modified (read-only)\",\n      \"readOnly\": true\n    },\n    \"phoneNumber\": {\n      \"type\": \"string\",\n      \"maxLength\": 30,\n      \"description\": \"The phone number associated with the order\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"maxLength\": 80,\n      \"format\": \"email\",\n      \"description\": \"The email address associated with the order\"\n    },\n    \"salesOrderLines\": {\n      \"type\": \"array\",\n      \"description\": \"The line items on the sales order\",\n      \"items\": {\n        \"$ref\": \"sales-order-line.json\"\n      }\n    }\n  },\n  \"required\": [\"id\"],\n  \"additionalProperties\": false,\n  \"$defs\": {\n    \"SalesOrderLine\": {\n      \"$id\": \"sales-order-line.json\"\
  ,\n      \"title\": \"Sales Order Line\",\n      \"description\": \"Represents a line item on a sales order, specifying the item, quantity, pricing, and shipping details.\",\n      \"type\": \"object\",\n      \"properties\": {\n        \"@odata.etag\": {\n          \"type\": \"string\",\n          \"description\": \"ETag for concurrency control\"\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The unique identifier of the sales order line\"\n        },\n        \"documentId\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The ID of the parent sales order document\"\n        },\n        \"sequence\": {\n          \"type\": \"integer\",\n          \"description\": \"The sequence number determining line order\"\n        },\n        \"itemId\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The unique identifier\
  \ of the item on this line\"\n        },\n        \"accountId\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The unique identifier of the G/L account (for account-type lines)\"\n        },\n        \"lineType\": {\n          \"type\": \"string\",\n          \"enum\": [\"Comment\", \"Account\", \"Item\", \"Resource\", \"Fixed Asset\", \"Charge\"],\n          \"description\": \"The type of the sales order line\"\n        },\n        \"lineObjectNumber\": {\n          \"type\": \"string\",\n          \"maxLength\": 20,\n          \"description\": \"The number of the item, account, resource, or asset on the line\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"maxLength\": 100,\n          \"description\": \"The description of the line item\"\n        },\n        \"description2\": {\n          \"type\": \"string\",\n          \"maxLength\": 50,\n          \"description\": \"Additional description for\
  \ the line item\"\n        },\n        \"unitOfMeasureId\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The unique identifier of the unit of measure\"\n        },\n        \"unitOfMeasureCode\": {\n          \"type\": \"string\",\n          \"maxLength\": 10,\n          \"description\": \"The unit of measure code (e.g., PCS, KG)\"\n        },\n        \"quantity\": {\n          \"type\": \"number\",\n          \"description\": \"The quantity ordered\"\n        },\n        \"unitPrice\": {\n          \"type\": \"number\",\n          \"description\": \"The unit selling price\"\n        },\n        \"discountAmount\": {\n          \"type\": \"number\",\n          \"description\": \"The line discount amount\"\n        },\n        \"discountPercent\": {\n          \"type\": \"number\",\n          \"description\": \"The line discount percentage\"\n        },\n        \"discountAppliedBeforeTax\": {\n          \"type\": \"boolean\",\n    \
  \      \"description\": \"Indicates whether the discount is applied before tax\"\n        },\n        \"amountExcludingTax\": {\n          \"type\": \"number\",\n          \"description\": \"The line amount excluding tax (read-only)\",\n          \"readOnly\": true\n        },\n        \"taxCode\": {\n          \"type\": \"string\",\n          \"maxLength\": 20,\n          \"description\": \"The tax code applied to the line\"\n        },\n        \"taxPercent\": {\n          \"type\": \"number\",\n          \"description\": \"The tax percentage (read-only)\",\n          \"readOnly\": true\n        },\n        \"totalTaxAmount\": {\n          \"type\": \"number\",\n          \"description\": \"The total tax amount for the line (read-only)\",\n          \"readOnly\": true\n        },\n        \"amountIncludingTax\": {\n          \"type\": \"number\",\n          \"description\": \"The line amount including tax (read-only)\",\n          \"readOnly\": true\n        },\n        \"netAmount\"\
  : {\n          \"type\": \"number\",\n          \"description\": \"The net amount (read-only)\",\n          \"readOnly\": true\n        },\n        \"netTaxAmount\": {\n          \"type\": \"number\",\n          \"description\": \"The net tax amount (read-only)\",\n          \"readOnly\": true\n        },\n        \"netAmountIncludingTax\": {\n          \"type\": \"number\",\n          \"description\": \"The net amount including tax (read-only)\",\n          \"readOnly\": true\n        },\n        \"shipmentDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"The planned shipment date for the line\"\n        },\n        \"shippedQuantity\": {\n          \"type\": \"number\",\n          \"description\": \"The quantity already shipped (read-only)\",\n          \"readOnly\": true\n        },\n        \"invoicedQuantity\": {\n          \"type\": \"number\",\n          \"description\": \"The quantity already invoiced (read-only)\",\n    \
  \      \"readOnly\": true\n        },\n        \"invoiceQuantity\": {\n          \"type\": \"number\",\n          \"description\": \"The quantity to invoice\"\n        },\n        \"shipQuantity\": {\n          \"type\": \"number\",\n          \"description\": \"The quantity to ship\"\n        }\n      },\n      \"required\": [\"id\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/sales-order.json
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
title: Sales Order
---
