---
description: Represents a purchase order entity in Dynamics 365 Business Central. Purchase orders are documents used to record the purchase of goods or services from vendors. They include header information (vendor, dates, payment terms) and line items specifying the products or services being purchased.
layout: schema
name: Purchase Order
properties_list:
- description: ETag for optimistic concurrency control
  name: '@odata.etag'
  type: string
- description: The unique identifier (GUID) of the purchase order
  name: id
  type: string
- description: The purchase order number assigned from a number series
  name: number
  type: string
- description: The date when the purchase order was created
  name: orderDate
  type: string
- description: The date used for posting the purchase order to the general ledger
  name: postingDate
  type: string
- description: The unique identifier of the buy-from vendor
  name: vendorId
  type: string
- description: The vendor number of the buy-from vendor
  name: vendorNumber
  type: string
- description: The name of the buy-from vendor
  name: vendorName
  type: string
- description: The name of the pay-to party
  name: payToName
  type: string
- description: The unique identifier of the pay-to vendor
  name: payToVendorId
  type: string
- description: The vendor number of the pay-to vendor
  name: payToVendorNumber
  type: string
- description: The name for the ship-to (receiving) address
  name: shipToName
  type: string
- description: The contact person at the ship-to address
  name: shipToContact
  type: string
- description: First line of the buy-from vendor address
  name: buyFromAddressLine1
  type: string
- description: Second line of the buy-from vendor address
  name: buyFromAddressLine2
  type: string
- description: The city of the buy-from vendor address
  name: buyFromCity
  type: string
- description: The country/region code of the buy-from vendor address
  name: buyFromCountry
  type: string
- description: The state or province code of the buy-from vendor address
  name: buyFromState
  type: string
- description: The postal code of the buy-from vendor address
  name: buyFromPostCode
  type: string
- description: The unique identifier of the currency
  name: currencyId
  type: string
- description: The currency code (e.g., USD, EUR) for the purchase order
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
- description: The purchaser/buyer code assigned to the order
  name: purchaser
  type: string
- description: The date the goods are requested to be received
  name: requestedReceiptDate
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
- description: Indicates whether all lines on the order have been fully received (read-only)
  name: fullyReceived
  type: boolean
- description: The current status of the purchase order (read-only)
  name: status
  type: string
- description: The date and time the purchase order was last modified (read-only)
  name: lastModifiedDateTime
  type: string
- description: The line items on the purchase order
  name: purchaseOrderLines
  type: array
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/purchase-order.json
slug: purchase-order
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://example.com/schemas/navision/purchase-order.json\",\n  \"title\": \"Purchase Order\",\n  \"description\": \"Represents a purchase order entity in Dynamics 365 Business Central. Purchase orders are documents used to record the purchase of goods or services from vendors. They include header information (vendor, dates, payment terms) and line items specifying the products or services being purchased.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"@odata.etag\": {\n      \"type\": \"string\",\n      \"description\": \"ETag for optimistic concurrency control\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier (GUID) of the purchase order\"\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"maxLength\": 20,\n      \"description\": \"The purchase order number assigned from a number series\"\n\
  \    },\n    \"orderDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The date when the purchase order was created\"\n    },\n    \"postingDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The date used for posting the purchase order to the general ledger\"\n    },\n    \"vendorId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the buy-from vendor\"\n    },\n    \"vendorNumber\": {\n      \"type\": \"string\",\n      \"maxLength\": 20,\n      \"description\": \"The vendor number of the buy-from vendor\"\n    },\n    \"vendorName\": {\n      \"type\": \"string\",\n      \"maxLength\": 100,\n      \"description\": \"The name of the buy-from vendor\"\n    },\n    \"payToName\": {\n      \"type\": \"string\",\n      \"maxLength\": 100,\n      \"description\": \"The name of the pay-to party\"\n    },\n    \"payToVendorId\": {\n      \"type\"\
  : \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the pay-to vendor\"\n    },\n    \"payToVendorNumber\": {\n      \"type\": \"string\",\n      \"maxLength\": 20,\n      \"description\": \"The vendor number of the pay-to vendor\"\n    },\n    \"shipToName\": {\n      \"type\": \"string\",\n      \"maxLength\": 100,\n      \"description\": \"The name for the ship-to (receiving) address\"\n    },\n    \"shipToContact\": {\n      \"type\": \"string\",\n      \"maxLength\": 100,\n      \"description\": \"The contact person at the ship-to address\"\n    },\n    \"buyFromAddressLine1\": {\n      \"type\": \"string\",\n      \"maxLength\": 100,\n      \"description\": \"First line of the buy-from vendor address\"\n    },\n    \"buyFromAddressLine2\": {\n      \"type\": \"string\",\n      \"maxLength\": 50,\n      \"description\": \"Second line of the buy-from vendor address\"\n    },\n    \"buyFromCity\": {\n      \"type\": \"string\",\n      \"maxLength\"\
  : 30,\n      \"description\": \"The city of the buy-from vendor address\"\n    },\n    \"buyFromCountry\": {\n      \"type\": \"string\",\n      \"maxLength\": 10,\n      \"description\": \"The country/region code of the buy-from vendor address\"\n    },\n    \"buyFromState\": {\n      \"type\": \"string\",\n      \"maxLength\": 20,\n      \"description\": \"The state or province code of the buy-from vendor address\"\n    },\n    \"buyFromPostCode\": {\n      \"type\": \"string\",\n      \"maxLength\": 20,\n      \"description\": \"The postal code of the buy-from vendor address\"\n    },\n    \"currencyId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the currency\"\n    },\n    \"currencyCode\": {\n      \"type\": \"string\",\n      \"maxLength\": 10,\n      \"description\": \"The currency code (e.g., USD, EUR) for the purchase order\"\n    },\n    \"pricesIncludeTax\": {\n      \"type\": \"boolean\",\n      \"description\"\
  : \"Indicates whether the prices on the order include tax\"\n    },\n    \"paymentTermsId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the payment terms\"\n    },\n    \"shipmentMethodId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the shipment method\"\n    },\n    \"purchaser\": {\n      \"type\": \"string\",\n      \"maxLength\": 20,\n      \"description\": \"The purchaser/buyer code assigned to the order\"\n    },\n    \"requestedReceiptDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The date the goods are requested to be received\"\n    },\n    \"discountAmount\": {\n      \"type\": \"number\",\n      \"description\": \"The total invoice discount amount applied to the order\"\n    },\n    \"discountAppliedBeforeTax\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether discounts\
  \ are applied before tax calculation\"\n    },\n    \"totalAmountExcludingTax\": {\n      \"type\": \"number\",\n      \"description\": \"The total amount of the order excluding tax (read-only)\",\n      \"readOnly\": true\n    },\n    \"totalTaxAmount\": {\n      \"type\": \"number\",\n      \"description\": \"The total tax amount on the order (read-only)\",\n      \"readOnly\": true\n    },\n    \"totalAmountIncludingTax\": {\n      \"type\": \"number\",\n      \"description\": \"The total amount of the order including tax (read-only)\",\n      \"readOnly\": true\n    },\n    \"fullyReceived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether all lines on the order have been fully received (read-only)\",\n      \"readOnly\": true\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"Draft\", \"In Review\", \"Open\", \"Released\"],\n      \"description\": \"The current status of the purchase order (read-only)\",\n      \"readOnly\": true\n\
  \    },\n    \"lastModifiedDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the purchase order was last modified (read-only)\",\n      \"readOnly\": true\n    },\n    \"purchaseOrderLines\": {\n      \"type\": \"array\",\n      \"description\": \"The line items on the purchase order\",\n      \"items\": {\n        \"$ref\": \"purchase-order-line.json\"\n      }\n    }\n  },\n  \"required\": [\"id\"],\n  \"additionalProperties\": false,\n  \"$defs\": {\n    \"PurchaseOrderLine\": {\n      \"$id\": \"purchase-order-line.json\",\n      \"title\": \"Purchase Order Line\",\n      \"description\": \"Represents a line item on a purchase order, specifying the item, quantity, cost, and receipt details.\",\n      \"type\": \"object\",\n      \"properties\": {\n        \"@odata.etag\": {\n          \"type\": \"string\",\n          \"description\": \"ETag for concurrency control\"\n        },\n        \"id\": {\n          \"type\"\
  : \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The unique identifier of the purchase order line\"\n        },\n        \"documentId\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The ID of the parent purchase order document\"\n        },\n        \"sequence\": {\n          \"type\": \"integer\",\n          \"description\": \"The sequence number determining line order\"\n        },\n        \"itemId\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The unique identifier of the item on this line\"\n        },\n        \"accountId\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The unique identifier of the G/L account (for account-type lines)\"\n        },\n        \"lineType\": {\n          \"type\": \"string\",\n          \"enum\": [\"Comment\", \"Account\", \"Item\", \"Fixed Asset\", \"Charge\"],\n  \
  \        \"description\": \"The type of the purchase order line\"\n        },\n        \"lineObjectNumber\": {\n          \"type\": \"string\",\n          \"maxLength\": 20,\n          \"description\": \"The number of the item, account, or asset on the line\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"maxLength\": 100,\n          \"description\": \"The description of the line item\"\n        },\n        \"description2\": {\n          \"type\": \"string\",\n          \"maxLength\": 50,\n          \"description\": \"Additional description for the line item\"\n        },\n        \"unitOfMeasureId\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The unique identifier of the unit of measure\"\n        },\n        \"unitOfMeasureCode\": {\n          \"type\": \"string\",\n          \"maxLength\": 10,\n          \"description\": \"The unit of measure code (e.g., PCS, KG)\"\n        },\n        \"quantity\"\
  : {\n          \"type\": \"number\",\n          \"description\": \"The quantity ordered\"\n        },\n        \"directUnitCost\": {\n          \"type\": \"number\",\n          \"description\": \"The direct unit cost from the vendor\"\n        },\n        \"discountAmount\": {\n          \"type\": \"number\",\n          \"description\": \"The line discount amount\"\n        },\n        \"discountPercent\": {\n          \"type\": \"number\",\n          \"description\": \"The line discount percentage\"\n        },\n        \"discountAppliedBeforeTax\": {\n          \"type\": \"boolean\",\n          \"description\": \"Indicates whether the discount is applied before tax\"\n        },\n        \"amountExcludingTax\": {\n          \"type\": \"number\",\n          \"description\": \"The line amount excluding tax (read-only)\",\n          \"readOnly\": true\n        },\n        \"taxCode\": {\n          \"type\": \"string\",\n          \"maxLength\": 20,\n          \"description\": \"The tax\
  \ code applied to the line\"\n        },\n        \"taxPercent\": {\n          \"type\": \"number\",\n          \"description\": \"The tax percentage (read-only)\",\n          \"readOnly\": true\n        },\n        \"totalTaxAmount\": {\n          \"type\": \"number\",\n          \"description\": \"The total tax amount for the line (read-only)\",\n          \"readOnly\": true\n        },\n        \"amountIncludingTax\": {\n          \"type\": \"number\",\n          \"description\": \"The line amount including tax (read-only)\",\n          \"readOnly\": true\n        },\n        \"expectedReceiptDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"The expected date of receipt for the line\"\n        },\n        \"receivedQuantity\": {\n          \"type\": \"number\",\n          \"description\": \"The quantity already received (read-only)\",\n          \"readOnly\": true\n        },\n        \"invoicedQuantity\": {\n          \"type\"\
  : \"number\",\n          \"description\": \"The quantity already invoiced (read-only)\",\n          \"readOnly\": true\n        },\n        \"invoiceQuantity\": {\n          \"type\": \"number\",\n          \"description\": \"The quantity to invoice\"\n        },\n        \"receiveQuantity\": {\n          \"type\": \"number\",\n          \"description\": \"The quantity to receive\"\n        }\n      },\n      \"required\": [\"id\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/purchase-order.json
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
title: Purchase Order
---
