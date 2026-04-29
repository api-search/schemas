---
description: Schema representing a purchase order in Oracle E-Business Suite Purchasing module. Maps to PO_HEADERS_ALL, PO_LINES_ALL, PO_LINE_LOCATIONS_ALL, and PO_DISTRIBUTIONS_ALL tables.
layout: schema
name: Oracle EBS Purchase Order
properties_list:
- description: Unique identifier for the purchase order header (PO_HEADERS_ALL.PO_HEADER_ID)
  name: poHeaderId
  type: integer
- description: Purchase order number (PO_HEADERS_ALL.SEGMENT1)
  name: segment1
  type: string
- description: Purchase order type
  name: typeLookupCode
  type: string
- description: Document revision number
  name: revisionNum
  type: integer
- description: Supplier/vendor identifier (AP_SUPPLIERS.VENDOR_ID)
  name: vendorId
  type: integer
- description: Supplier/vendor name
  name: vendorName
  type: string
- description: Vendor site identifier (AP_SUPPLIER_SITES_ALL.VENDOR_SITE_ID)
  name: vendorSiteId
  type: integer
- description: Vendor site code
  name: vendorSiteCode
  type: string
- description: Vendor contact identifier
  name: vendorContactId
  type: integer
- description: Document currency code (ISO 4217)
  name: currencyCode
  type: string
- description: Currency exchange rate type
  name: rateType
  type:
  - string
  - 'null'
- description: Currency exchange rate
  name: rate
  type:
  - number
  - 'null'
- description: Exchange rate date
  name: rateDate
  type:
  - string
  - 'null'
- description: Buyer/agent employee identifier
  name: agentId
  type: integer
- description: Authorization/approval status of the purchase order
  name: authorizationStatus
  type: string
- description: Whether the PO has been approved
  name: approvedFlag
  type: string
- description: Date the purchase order was approved
  name: approvedDate
  type:
  - string
  - 'null'
- description: Close status of the purchase order
  name: closedCode
  type: string
- description: Date the purchase order was closed
  name: closedDate
  type:
  - string
  - 'null'
- description: Default ship-to location identifier (HR_LOCATIONS_ALL.LOCATION_ID)
  name: shipToLocationId
  type: integer
- description: Default bill-to location identifier
  name: billToLocationId
  type: integer
- description: Payment terms identifier (AP_TERMS.TERM_ID)
  name: termsId
  type: integer
- description: Purchase order description
  name: description
  type:
  - string
  - 'null'
- description: Purchase order comments
  name: comments
  type:
  - string
  - 'null'
- description: Total purchase order amount
  name: totalAmount
  type: number
- description: ''
  name: confirmedFlag
  type: string
- description: Number of times the PO has been printed
  name: printCount
  type: integer
- description: Purchase order lines
  name: lines
  type: array
- description: Operating unit identifier (HR_OPERATING_UNITS.ORGANIZATION_ID)
  name: orgId
  type: integer
- description: User who created the record (FND_USER.USER_ID)
  name: createdBy
  type: integer
- description: Record creation date
  name: creationDate
  type: string
- description: User who last updated the record
  name: lastUpdatedBy
  type: integer
- description: Record last update date
  name: lastUpdateDate
  type: string
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/purchase-order.json
slug: purchase-order
source_filename: purchase-order.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.oracle.com/ebs/purchase-order.json\",\n  \"title\": \"Oracle EBS Purchase Order\",\n  \"description\": \"Schema representing a purchase order in Oracle E-Business Suite Purchasing module. Maps to PO_HEADERS_ALL, PO_LINES_ALL, PO_LINE_LOCATIONS_ALL, and PO_DISTRIBUTIONS_ALL tables.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"poHeaderId\",\n    \"segment1\",\n    \"vendorId\",\n    \"currencyCode\"\n  ],\n  \"properties\": {\n    \"poHeaderId\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the purchase order header (PO_HEADERS_ALL.PO_HEADER_ID)\"\n    },\n    \"segment1\": {\n      \"type\": \"string\",\n      \"description\": \"Purchase order number (PO_HEADERS_ALL.SEGMENT1)\",\n      \"maxLength\": 20\n    },\n    \"typeLookupCode\": {\n      \"type\": \"string\",\n      \"description\": \"Purchase order type\",\n      \"enum\": [\n\
  \        \"STANDARD\",\n        \"BLANKET\",\n        \"CONTRACT\",\n        \"PLANNED\"\n      ]\n    },\n    \"revisionNum\": {\n      \"type\": \"integer\",\n      \"description\": \"Document revision number\",\n      \"minimum\": 0\n    },\n    \"vendorId\": {\n      \"type\": \"integer\",\n      \"description\": \"Supplier/vendor identifier (AP_SUPPLIERS.VENDOR_ID)\"\n    },\n    \"vendorName\": {\n      \"type\": \"string\",\n      \"description\": \"Supplier/vendor name\",\n      \"maxLength\": 240\n    },\n    \"vendorSiteId\": {\n      \"type\": \"integer\",\n      \"description\": \"Vendor site identifier (AP_SUPPLIER_SITES_ALL.VENDOR_SITE_ID)\"\n    },\n    \"vendorSiteCode\": {\n      \"type\": \"string\",\n      \"description\": \"Vendor site code\",\n      \"maxLength\": 15\n    },\n    \"vendorContactId\": {\n      \"type\": \"integer\",\n      \"description\": \"Vendor contact identifier\"\n    },\n    \"currencyCode\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Document currency code (ISO 4217)\",\n      \"pattern\": \"^[A-Z]{3}$\",\n      \"examples\": [\n        \"USD\",\n        \"EUR\",\n        \"GBP\"\n      ]\n    },\n    \"rateType\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Currency exchange rate type\"\n    },\n    \"rate\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Currency exchange rate\"\n    },\n    \"rateDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"Exchange rate date\"\n    },\n    \"agentId\": {\n      \"type\": \"integer\",\n      \"description\": \"Buyer/agent employee identifier\"\n    },\n    \"authorizationStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Authorization/approval status of the purchase order\",\n      \"enum\": [\n        \"APPROVED\",\n        \"IN PROCESS\",\n        \"INCOMPLETE\",\n        \"PRE-APPROVED\",\n        \"REJECTED\",\n        \"REQUIRES REAPPROVAL\"\n    \
  \  ]\n    },\n    \"approvedFlag\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the PO has been approved\",\n      \"enum\": [\n        \"Y\",\n        \"N\"\n      ]\n    },\n    \"approvedDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"Date the purchase order was approved\"\n    },\n    \"closedCode\": {\n      \"type\": \"string\",\n      \"description\": \"Close status of the purchase order\",\n      \"enum\": [\n        \"OPEN\",\n        \"CLOSED\",\n        \"FINALLY CLOSED\",\n        \"CLOSED FOR RECEIVING\",\n        \"CLOSED FOR INVOICE\"\n      ]\n    },\n    \"closedDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"Date the purchase order was closed\"\n    },\n    \"shipToLocationId\": {\n      \"type\": \"integer\",\n      \"description\": \"Default ship-to location identifier (HR_LOCATIONS_ALL.LOCATION_ID)\"\n    },\n    \"billToLocationId\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"Default bill-to location identifier\"\n    },\n    \"termsId\": {\n      \"type\": \"integer\",\n      \"description\": \"Payment terms identifier (AP_TERMS.TERM_ID)\"\n    },\n    \"description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Purchase order description\",\n      \"maxLength\": 240\n    },\n    \"comments\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Purchase order comments\"\n    },\n    \"totalAmount\": {\n      \"type\": \"number\",\n      \"description\": \"Total purchase order amount\",\n      \"minimum\": 0\n    },\n    \"confirmedFlag\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Y\",\n        \"N\"\n      ]\n    },\n    \"printCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of times the PO has been printed\",\n      \"minimum\": 0\n    },\n    \"lines\": {\n      \"type\": \"array\",\n      \"description\": \"\
  Purchase order lines\",\n      \"items\": {\n        \"$ref\": \"#/$defs/PurchaseOrderLine\"\n      }\n    },\n    \"orgId\": {\n      \"type\": \"integer\",\n      \"description\": \"Operating unit identifier (HR_OPERATING_UNITS.ORGANIZATION_ID)\"\n    },\n    \"createdBy\": {\n      \"type\": \"integer\",\n      \"description\": \"User who created the record (FND_USER.USER_ID)\"\n    },\n    \"creationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Record creation date\"\n    },\n    \"lastUpdatedBy\": {\n      \"type\": \"integer\",\n      \"description\": \"User who last updated the record\"\n    },\n    \"lastUpdateDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Record last update date\"\n    }\n  },\n  \"$defs\": {\n    \"PurchaseOrderLine\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"poLineId\",\n        \"lineNum\"\n      ],\n      \"properties\": {\n    \
  \    \"poLineId\": {\n          \"type\": \"integer\",\n          \"description\": \"Purchase order line identifier (PO_LINES_ALL.PO_LINE_ID)\"\n        },\n        \"lineNum\": {\n          \"type\": \"integer\",\n          \"description\": \"Line number\",\n          \"minimum\": 1\n        },\n        \"lineTypeId\": {\n          \"type\": \"integer\",\n          \"description\": \"Line type identifier\"\n        },\n        \"itemId\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"Inventory item identifier (MTL_SYSTEM_ITEMS_B.INVENTORY_ITEM_ID)\"\n        },\n        \"itemDescription\": {\n          \"type\": \"string\",\n          \"description\": \"Item description\",\n          \"maxLength\": 240\n        },\n        \"itemRevision\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Item revision\"\n        },\n        \"categoryId\": {\n          \"type\": \"integer\",\n          \"description\": \"Purchasing category\
  \ identifier\"\n        },\n        \"quantity\": {\n          \"type\": \"number\",\n          \"description\": \"Ordered quantity\",\n          \"minimum\": 0\n        },\n        \"unitMeasLookupCode\": {\n          \"type\": \"string\",\n          \"description\": \"Unit of measure lookup code\",\n          \"maxLength\": 25\n        },\n        \"unitPrice\": {\n          \"type\": \"number\",\n          \"description\": \"Unit price\",\n          \"minimum\": 0\n        },\n        \"amount\": {\n          \"type\": \"number\",\n          \"description\": \"Line amount (quantity * unitPrice)\"\n        },\n        \"closedCode\": {\n          \"type\": \"string\",\n          \"description\": \"Line close status\",\n          \"enum\": [\n            \"OPEN\",\n            \"CLOSED\",\n            \"FINALLY CLOSED\",\n            \"CLOSED FOR RECEIVING\",\n            \"CLOSED FOR INVOICE\"\n          ]\n        },\n        \"cancelFlag\": {\n          \"type\": \"string\",\n    \
  \      \"description\": \"Whether the line is cancelled\",\n          \"enum\": [\n            \"Y\",\n            \"N\"\n          ]\n        },\n        \"vendorProductNum\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Vendor product number\",\n          \"maxLength\": 25\n        },\n        \"needByDate\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date\",\n          \"description\": \"Need-by date\"\n        },\n        \"promisedDate\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date\",\n          \"description\": \"Promised delivery date\"\n        },\n        \"noteToVendor\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Note to vendor for this line\"\n        },\n        \"shipments\": {\n          \"type\": \"array\",\n          \"description\": \"Line location/shipment records\",\n          \"items\": {\n            \"$ref\": \"#/$defs/PurchaseOrderShipment\"\
  \n          }\n        },\n        \"creationDate\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"lastUpdateDate\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        }\n      }\n    },\n    \"PurchaseOrderShipment\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"lineLocationId\",\n        \"shipmentNum\"\n      ],\n      \"properties\": {\n        \"lineLocationId\": {\n          \"type\": \"integer\",\n          \"description\": \"Line location/shipment identifier (PO_LINE_LOCATIONS_ALL.LINE_LOCATION_ID)\"\n        },\n        \"shipmentNum\": {\n          \"type\": \"integer\",\n          \"description\": \"Shipment number\",\n          \"minimum\": 1\n        },\n        \"quantity\": {\n          \"type\": \"number\",\n          \"description\": \"Shipment quantity\",\n          \"minimum\": 0\n        },\n        \"quantityReceived\": {\n          \"type\": \"number\",\n          \"\
  description\": \"Quantity received to date\",\n          \"minimum\": 0\n        },\n        \"quantityAccepted\": {\n          \"type\": \"number\",\n          \"description\": \"Quantity accepted\",\n          \"minimum\": 0\n        },\n        \"quantityRejected\": {\n          \"type\": \"number\",\n          \"description\": \"Quantity rejected\",\n          \"minimum\": 0\n        },\n        \"quantityBilled\": {\n          \"type\": \"number\",\n          \"description\": \"Quantity billed/invoiced\",\n          \"minimum\": 0\n        },\n        \"quantityCancelled\": {\n          \"type\": \"number\",\n          \"description\": \"Quantity cancelled\",\n          \"minimum\": 0\n        },\n        \"needByDate\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date\"\n        },\n        \"promisedDate\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date\"\n        },\n        \"shipToOrganizationId\": {\n          \"type\"\
  : \"integer\",\n          \"description\": \"Ship-to organization identifier\"\n        },\n        \"shipToLocationId\": {\n          \"type\": \"integer\",\n          \"description\": \"Ship-to location identifier\"\n        },\n        \"closedCode\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"OPEN\",\n            \"CLOSED\",\n            \"FINALLY CLOSED\",\n            \"CLOSED FOR RECEIVING\",\n            \"CLOSED FOR INVOICE\"\n          ]\n        },\n        \"distributions\": {\n          \"type\": \"array\",\n          \"description\": \"Distribution records\",\n          \"items\": {\n            \"$ref\": \"#/$defs/PurchaseOrderDistribution\"\n          }\n        }\n      }\n    },\n    \"PurchaseOrderDistribution\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"poDistributionId\",\n        \"distributionNum\"\n      ],\n      \"properties\": {\n        \"poDistributionId\": {\n          \"type\": \"integer\",\n          \"\
  description\": \"Distribution identifier (PO_DISTRIBUTIONS_ALL.PO_DISTRIBUTION_ID)\"\n        },\n        \"distributionNum\": {\n          \"type\": \"integer\",\n          \"description\": \"Distribution number\",\n          \"minimum\": 1\n        },\n        \"quantity\": {\n          \"type\": \"number\",\n          \"description\": \"Distribution quantity\"\n        },\n        \"quantityDelivered\": {\n          \"type\": \"number\",\n          \"description\": \"Quantity delivered\"\n        },\n        \"quantityBilled\": {\n          \"type\": \"number\",\n          \"description\": \"Quantity billed\"\n        },\n        \"codeCombinatonId\": {\n          \"type\": \"integer\",\n          \"description\": \"Charge account code combination ID (GL_CODE_COMBINATIONS.CODE_COMBINATION_ID)\"\n        },\n        \"setOfBooksId\": {\n          \"type\": \"integer\",\n          \"description\": \"Set of books/ledger identifier\"\n        },\n        \"destinationTypeCode\": {\n   \
  \       \"type\": \"string\",\n          \"description\": \"Destination type\",\n          \"enum\": [\n            \"INVENTORY\",\n            \"EXPENSE\",\n            \"SHOP FLOOR\"\n          ]\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/purchase-order.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: Oracle EBS Purchase Order
---
