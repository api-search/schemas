---
description: A tax transaction represents a taxable event such as a sale, purchase, or return processed through the AvaTax API. It contains header-level information, line items, calculated tax amounts, and jurisdiction details.
layout: schema
name: Avalara Tax Transaction
properties_list:
- description: Unique identifier for the transaction
  name: id
  type: integer
- description: Unique transaction code assigned by the client or auto-generated
  name: code
  type: string
- description: Code identifying the company that owns this transaction
  name: companyCode
  type: string
- description: The document type for this transaction
  name: type
  type: string
- description: Current lifecycle status of the transaction
  name: status
  type: string
- description: Date of the transaction
  name: date
  type: string
- description: Unique code identifying the customer for this transaction
  name: customerCode
  type: string
- description: Three-character ISO 4217 currency code
  name: currencyCode
  type: string
- description: Whether the transaction should be committed immediately
  name: commit
  type: boolean
- description: Total amount of the transaction before tax
  name: totalAmount
  type: number
- description: Total tax calculated for the transaction
  name: totalTax
  type: number
- description: Total taxable amount
  name: totalTaxable
  type: number
- description: Total exempt amount
  name: totalExempt
  type: number
- description: Total discount applied
  name: totalDiscount
  type: number
- description: Total tax calculated before any adjustments
  name: totalTaxCalculated
  type: number
- description: Address information for the transaction
  name: addresses
  type: object
- description: Line items included in this transaction
  name: lines
  type: array
- description: Tax summary broken down by jurisdiction
  name: summary
  type: array
- description: Date and time the transaction was created
  name: createdDate
  type: string
- description: Date and time the transaction was last modified
  name: modifiedDate
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avalara-transaction-schema.json
slug: avalara-transaction
source_filename: avalara-transaction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.avalara.com/schemas/avalara/transaction.json\",\n  \"title\": \"Avalara Tax Transaction\",\n  \"description\": \"A tax transaction represents a taxable event such as a sale, purchase, or return processed through the AvaTax API. It contains header-level information, line items, calculated tax amounts, and jurisdiction details.\",\n  \"type\": \"object\",\n  \"required\": [\"type\", \"companyCode\", \"date\", \"customerCode\", \"lines\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the transaction\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Unique transaction code assigned by the client or auto-generated\"\n    },\n    \"companyCode\": {\n      \"type\": \"string\",\n      \"description\": \"Code identifying the company that owns this transaction\"\n    },\n    \"type\":\
  \ {\n      \"type\": \"string\",\n      \"enum\": [\"SalesOrder\", \"SalesInvoice\", \"PurchaseOrder\", \"PurchaseInvoice\", \"ReturnOrder\", \"ReturnInvoice\"],\n      \"description\": \"The document type for this transaction\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"Temporary\", \"Saved\", \"Posted\", \"Committed\", \"Cancelled\", \"Adjusted\"],\n      \"description\": \"Current lifecycle status of the transaction\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of the transaction\"\n    },\n    \"customerCode\": {\n      \"type\": \"string\",\n      \"description\": \"Unique code identifying the customer for this transaction\"\n    },\n    \"currencyCode\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[A-Z]{3}$\",\n      \"description\": \"Three-character ISO 4217 currency code\"\n    },\n    \"commit\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"\
  description\": \"Whether the transaction should be committed immediately\"\n    },\n    \"totalAmount\": {\n      \"type\": \"number\",\n      \"description\": \"Total amount of the transaction before tax\"\n    },\n    \"totalTax\": {\n      \"type\": \"number\",\n      \"description\": \"Total tax calculated for the transaction\"\n    },\n    \"totalTaxable\": {\n      \"type\": \"number\",\n      \"description\": \"Total taxable amount\"\n    },\n    \"totalExempt\": {\n      \"type\": \"number\",\n      \"description\": \"Total exempt amount\"\n    },\n    \"totalDiscount\": {\n      \"type\": \"number\",\n      \"description\": \"Total discount applied\"\n    },\n    \"totalTaxCalculated\": {\n      \"type\": \"number\",\n      \"description\": \"Total tax calculated before any adjustments\"\n    },\n    \"addresses\": {\n      \"type\": \"object\",\n      \"description\": \"Address information for the transaction\",\n      \"properties\": {\n        \"shipFrom\": {\n          \"\
  $ref\": \"#/$defs/Address\"\n        },\n        \"shipTo\": {\n          \"$ref\": \"#/$defs/Address\"\n        },\n        \"pointOfOrderOrigin\": {\n          \"$ref\": \"#/$defs/Address\"\n        },\n        \"pointOfOrderAcceptance\": {\n          \"$ref\": \"#/$defs/Address\"\n        }\n      }\n    },\n    \"lines\": {\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/$defs/TransactionLine\"\n      },\n      \"description\": \"Line items included in this transaction\"\n    },\n    \"summary\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/TaxSummary\"\n      },\n      \"description\": \"Tax summary broken down by jurisdiction\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the transaction was created\"\n    },\n    \"modifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"Date and time the transaction was last modified\"\n    }\n  },\n  \"$defs\": {\n    \"Address\": {\n      \"type\": \"object\",\n      \"description\": \"A physical address used for tax jurisdiction determination\",\n      \"properties\": {\n        \"line1\": {\n          \"type\": \"string\",\n          \"description\": \"Street address line 1\"\n        },\n        \"line2\": {\n          \"type\": \"string\",\n          \"description\": \"Street address line 2\"\n        },\n        \"line3\": {\n          \"type\": \"string\",\n          \"description\": \"Street address line 3\"\n        },\n        \"city\": {\n          \"type\": \"string\",\n          \"description\": \"City name\"\n        },\n        \"region\": {\n          \"type\": \"string\",\n          \"description\": \"State, province, or region code\"\n        },\n        \"postalCode\": {\n          \"type\": \"string\",\n          \"description\": \"Postal code or ZIP code\"\n        },\n        \"country\": {\n\
  \          \"type\": \"string\",\n          \"pattern\": \"^[A-Z]{2}$\",\n          \"description\": \"Two-character ISO 3166 country code\"\n        },\n        \"latitude\": {\n          \"type\": \"number\",\n          \"minimum\": -90,\n          \"maximum\": 90\n        },\n        \"longitude\": {\n          \"type\": \"number\",\n          \"minimum\": -180,\n          \"maximum\": 180\n        }\n      }\n    },\n    \"TransactionLine\": {\n      \"type\": \"object\",\n      \"description\": \"A single line item within a tax transaction\",\n      \"required\": [\"amount\"],\n      \"properties\": {\n        \"number\": {\n          \"type\": \"string\",\n          \"description\": \"Line number within the transaction\"\n        },\n        \"quantity\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"default\": 1,\n          \"description\": \"Quantity of items\"\n        },\n        \"amount\": {\n          \"type\": \"number\",\n          \"description\"\
  : \"Total amount for this line\"\n        },\n        \"taxCode\": {\n          \"type\": \"string\",\n          \"description\": \"Avalara tax code for this line item\"\n        },\n        \"itemCode\": {\n          \"type\": \"string\",\n          \"description\": \"Product or service item code\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Description of the line item\"\n        },\n        \"discountAmount\": {\n          \"type\": \"number\",\n          \"description\": \"Discount amount applied to this line\"\n        },\n        \"exemptionCode\": {\n          \"type\": \"string\",\n          \"description\": \"Exemption code for tax-exempt purchases\"\n        },\n        \"tax\": {\n          \"type\": \"number\",\n          \"description\": \"Calculated tax for this line\"\n        },\n        \"taxableAmount\": {\n          \"type\": \"number\",\n          \"description\": \"Taxable amount after exemptions\"\n      \
  \  },\n        \"exemptAmount\": {\n          \"type\": \"number\",\n          \"description\": \"Amount exempt from tax\"\n        },\n        \"addresses\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"shipFrom\": {\n              \"$ref\": \"#/$defs/Address\"\n            },\n            \"shipTo\": {\n              \"$ref\": \"#/$defs/Address\"\n            }\n          }\n        }\n      }\n    },\n    \"TaxSummary\": {\n      \"type\": \"object\",\n      \"description\": \"Tax calculation summary for a specific jurisdiction\",\n      \"properties\": {\n        \"country\": {\n          \"type\": \"string\",\n          \"description\": \"Country code\"\n        },\n        \"region\": {\n          \"type\": \"string\",\n          \"description\": \"State or province code\"\n        },\n        \"jurisType\": {\n          \"type\": \"string\",\n          \"enum\": [\"Country\", \"State\", \"County\", \"City\", \"Special\"],\n          \"description\"\
  : \"Jurisdiction type\"\n        },\n        \"jurisCode\": {\n          \"type\": \"string\",\n          \"description\": \"Jurisdiction code\"\n        },\n        \"jurisName\": {\n          \"type\": \"string\",\n          \"description\": \"Jurisdiction name\"\n        },\n        \"taxType\": {\n          \"type\": \"string\",\n          \"description\": \"Type of tax (e.g., Sales, Use, VAT)\"\n        },\n        \"rate\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"maximum\": 1,\n          \"description\": \"Tax rate as a decimal\"\n        },\n        \"tax\": {\n          \"type\": \"number\",\n          \"description\": \"Tax amount for this jurisdiction\"\n        },\n        \"taxable\": {\n          \"type\": \"number\",\n          \"description\": \"Taxable amount in this jurisdiction\"\n        },\n        \"exempt\": {\n          \"type\": \"number\",\n          \"description\": \"Exempt amount in this jurisdiction\"\n        }\n      }\n\
  \    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avalara-transaction-schema.json
tags:
- Taxes
title: Avalara Tax Transaction
---
