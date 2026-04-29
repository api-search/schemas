---
description: An Invoice represents a sales form where the customer pays for a product or service later. QuickBooks Online records an accounts receivable transaction for each invoice. This schema describes the full Invoice entity as returned by the QuickBooks Online Accounting API.
layout: schema
name: QuickBooks Online Invoice
properties_list:
- description: Unique identifier for the invoice, assigned by QuickBooks Online.
  name: Id
  type: string
- description: Version number of the entity used for optimistic concurrency control. Required for update operations. The value changes each time the entity is updated.
  name: SyncToken
  type: string
- description: ''
  name: MetaData
  type: object
- description: Reference number for the transaction. If not provided during creation, QuickBooks auto-generates a sequential number.
  name: DocNumber
  type: string
- description: The date of the transaction in YYYY-MM-DD format. Defaults to the current date if not specified.
  name: TxnDate
  type: string
- description: The date when payment is due. Calculated based on the sales terms if not explicitly set.
  name: DueDate
  type: string
- description: A private note for internal use that is not displayed to the customer.
  name: PrivateNote
  type: string
- description: A note to the customer that appears on the invoice.
  name: CustomerMemo
  type: object
- description: Reference to the customer associated with this invoice. Required for creation.
  name: CustomerRef
  type: object
- description: Bill-to address for the invoice.
  name: BillAddr
  type: object
- description: Ship-to address for the invoice.
  name: ShipAddr
  type: object
- description: Email address to which the invoice is sent.
  name: BillEmail
  type: object
- description: Individual line items of the transaction. At least one line item with a valid DetailType is required.
  name: Line
  type: array
- description: Tax details for the entire invoice transaction.
  name: TxnTaxDetail
  type: object
- description: Total amount of the transaction including tax. This is a calculated field and is read-only.
  name: TotalAmt
  type: number
- description: The balance remaining to be paid on the invoice. A value of 0 indicates the invoice is fully paid.
  name: Balance
  type: number
- description: Deposit amount previously applied to this invoice.
  name: Deposit
  type: number
- description: Account where the deposit was made.
  name: DepositToAccountRef
  type: object
- description: Reference to the sales term (e.g., Net 30, Due on Receipt).
  name: SalesTermRef
  type: object
- description: Reference to the payment method for this invoice.
  name: PaymentMethodRef
  type: object
- description: Reference to the currency used for this invoice. Only applicable for companies with multicurrency enabled.
  name: CurrencyRef
  type: object
- description: The exchange rate between the invoice currency and the home currency. Only applicable for multicurrency companies.
  name: ExchangeRate
  type: number
- description: Date for delivery of goods or services.
  name: ShipDate
  type: string
- description: Reference to the shipping method.
  name: ShipMethodRef
  type: object
- description: Shipping tracking number.
  name: TrackingNum
  type: string
- description: If true, tax is calculated after applying any discount. If false, tax is calculated before the discount.
  name: ApplyTaxAfterDiscount
  type: boolean
- description: Printing status of the invoice.
  name: PrintStatus
  type: string
- description: Email delivery status of the invoice.
  name: EmailStatus
  type: string
- description: Method in which tax is applied. TaxExcluded means line amounts are exclusive of tax. TaxInclusive means line amounts include tax.
  name: GlobalTaxCalculation
  type: string
- description: Whether online payment is allowed for this invoice.
  name: AllowOnlinePayment
  type: boolean
- description: Whether online credit card payment is allowed.
  name: AllowOnlineCreditCardPayment
  type: boolean
- description: Whether online ACH (bank transfer) payment is allowed.
  name: AllowOnlineACHPayment
  type: boolean
- description: Custom fields defined for the invoice. A maximum of 3 custom fields are supported.
  name: CustomField
  type: array
- description: Transactions linked to this invoice such as payments or credit memos.
  name: LinkedTxn
  type: array
- description: Domain of the entity (e.g., QBO).
  name: domain
  type: string
- description: Indicates whether this is a sparse (partial) representation of the entity.
  name: sparse
  type: boolean
provider_name: Intuit
provider_slug: intuit
schema_file: json-schema/intuit-invoice-schema.json
slug: intuit-invoice
source_filename: intuit-invoice-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/intuit/json-schema/intuit-invoice-schema.json\",\n  \"title\": \"QuickBooks Online Invoice\",\n  \"description\": \"An Invoice represents a sales form where the customer pays for a product or service later. QuickBooks Online records an accounts receivable transaction for each invoice. This schema describes the full Invoice entity as returned by the QuickBooks Online Accounting API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the invoice, assigned by QuickBooks Online.\",\n      \"readOnly\": true\n    },\n    \"SyncToken\": {\n      \"type\": \"string\",\n      \"description\": \"Version number of the entity used for optimistic concurrency control. Required for update operations. The value changes each time the entity is updated.\"\n    },\n    \"MetaData\": {\n  \
  \    \"$ref\": \"#/$defs/MetaData\"\n    },\n    \"DocNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Reference number for the transaction. If not provided during creation, QuickBooks auto-generates a sequential number.\",\n      \"maxLength\": 21\n    },\n    \"TxnDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The date of the transaction in YYYY-MM-DD format. Defaults to the current date if not specified.\"\n    },\n    \"DueDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The date when payment is due. Calculated based on the sales terms if not explicitly set.\"\n    },\n    \"PrivateNote\": {\n      \"type\": \"string\",\n      \"description\": \"A private note for internal use that is not displayed to the customer.\",\n      \"maxLength\": 4000\n    },\n    \"CustomerMemo\": {\n      \"type\": \"object\",\n      \"description\": \"A note to the customer that appears on the\
  \ invoice.\",\n      \"properties\": {\n        \"value\": {\n          \"type\": \"string\",\n          \"maxLength\": 1000\n        }\n      }\n    },\n    \"CustomerRef\": {\n      \"$ref\": \"#/$defs/ReferenceType\",\n      \"description\": \"Reference to the customer associated with this invoice. Required for creation.\"\n    },\n    \"BillAddr\": {\n      \"$ref\": \"#/$defs/PhysicalAddress\",\n      \"description\": \"Bill-to address for the invoice.\"\n    },\n    \"ShipAddr\": {\n      \"$ref\": \"#/$defs/PhysicalAddress\",\n      \"description\": \"Ship-to address for the invoice.\"\n    },\n    \"BillEmail\": {\n      \"$ref\": \"#/$defs/EmailAddress\",\n      \"description\": \"Email address to which the invoice is sent.\"\n    },\n    \"Line\": {\n      \"type\": \"array\",\n      \"description\": \"Individual line items of the transaction. At least one line item with a valid DetailType is required.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/InvoiceLine\"\n      },\n\
  \      \"minItems\": 1\n    },\n    \"TxnTaxDetail\": {\n      \"$ref\": \"#/$defs/TxnTaxDetail\",\n      \"description\": \"Tax details for the entire invoice transaction.\"\n    },\n    \"TotalAmt\": {\n      \"type\": \"number\",\n      \"description\": \"Total amount of the transaction including tax. This is a calculated field and is read-only.\",\n      \"readOnly\": true\n    },\n    \"Balance\": {\n      \"type\": \"number\",\n      \"description\": \"The balance remaining to be paid on the invoice. A value of 0 indicates the invoice is fully paid.\",\n      \"readOnly\": true\n    },\n    \"Deposit\": {\n      \"type\": \"number\",\n      \"description\": \"Deposit amount previously applied to this invoice.\"\n    },\n    \"DepositToAccountRef\": {\n      \"$ref\": \"#/$defs/ReferenceType\",\n      \"description\": \"Account where the deposit was made.\"\n    },\n    \"SalesTermRef\": {\n      \"$ref\": \"#/$defs/ReferenceType\",\n      \"description\": \"Reference to the sales\
  \ term (e.g., Net 30, Due on Receipt).\"\n    },\n    \"PaymentMethodRef\": {\n      \"$ref\": \"#/$defs/ReferenceType\",\n      \"description\": \"Reference to the payment method for this invoice.\"\n    },\n    \"CurrencyRef\": {\n      \"$ref\": \"#/$defs/ReferenceType\",\n      \"description\": \"Reference to the currency used for this invoice. Only applicable for companies with multicurrency enabled.\"\n    },\n    \"ExchangeRate\": {\n      \"type\": \"number\",\n      \"description\": \"The exchange rate between the invoice currency and the home currency. Only applicable for multicurrency companies.\"\n    },\n    \"ShipDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date for delivery of goods or services.\"\n    },\n    \"ShipMethodRef\": {\n      \"$ref\": \"#/$defs/ReferenceType\",\n      \"description\": \"Reference to the shipping method.\"\n    },\n    \"TrackingNum\": {\n      \"type\": \"string\",\n      \"description\": \"Shipping\
  \ tracking number.\"\n    },\n    \"ApplyTaxAfterDiscount\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, tax is calculated after applying any discount. If false, tax is calculated before the discount.\"\n    },\n    \"PrintStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Printing status of the invoice.\",\n      \"enum\": [\"NotSet\", \"NeedToPrint\", \"PrintComplete\"]\n    },\n    \"EmailStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Email delivery status of the invoice.\",\n      \"enum\": [\"NotSet\", \"NeedToSend\", \"EmailSent\"]\n    },\n    \"GlobalTaxCalculation\": {\n      \"type\": \"string\",\n      \"description\": \"Method in which tax is applied. TaxExcluded means line amounts are exclusive of tax. TaxInclusive means line amounts include tax.\",\n      \"enum\": [\"TaxExcluded\", \"TaxInclusive\", \"NotApplicable\"]\n    },\n    \"AllowOnlinePayment\": {\n      \"type\": \"boolean\",\n      \"description\": \"\
  Whether online payment is allowed for this invoice.\"\n    },\n    \"AllowOnlineCreditCardPayment\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether online credit card payment is allowed.\"\n    },\n    \"AllowOnlineACHPayment\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether online ACH (bank transfer) payment is allowed.\"\n    },\n    \"CustomField\": {\n      \"type\": \"array\",\n      \"description\": \"Custom fields defined for the invoice. A maximum of 3 custom fields are supported.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/CustomField\"\n      },\n      \"maxItems\": 3\n    },\n    \"LinkedTxn\": {\n      \"type\": \"array\",\n      \"description\": \"Transactions linked to this invoice such as payments or credit memos.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/LinkedTxn\"\n      }\n    },\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"Domain of the entity (e.g., QBO).\",\n      \"readOnly\": true\n\
  \    },\n    \"sparse\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether this is a sparse (partial) representation of the entity.\"\n    }\n  },\n  \"required\": [\"CustomerRef\", \"Line\"],\n  \"$defs\": {\n    \"ReferenceType\": {\n      \"type\": \"object\",\n      \"description\": \"A reference to another entity in QuickBooks Online, containing the entity ID and optionally a display name.\",\n      \"properties\": {\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of the referenced entity.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"An identifying name for the referenced entity.\"\n        }\n      },\n      \"required\": [\"value\"]\n    },\n    \"PhysicalAddress\": {\n      \"type\": \"object\",\n      \"description\": \"A physical (mailing) address.\",\n      \"properties\": {\n        \"Id\": {\n          \"type\": \"string\",\n          \"\
  description\": \"Unique identifier for the address.\"\n        },\n        \"Line1\": {\n          \"type\": \"string\",\n          \"description\": \"First line of the street address.\",\n          \"maxLength\": 500\n        },\n        \"Line2\": {\n          \"type\": \"string\",\n          \"description\": \"Second line of the street address.\",\n          \"maxLength\": 500\n        },\n        \"Line3\": {\n          \"type\": \"string\",\n          \"description\": \"Third line of the street address.\",\n          \"maxLength\": 500\n        },\n        \"Line4\": {\n          \"type\": \"string\",\n          \"description\": \"Fourth line of the street address.\",\n          \"maxLength\": 500\n        },\n        \"Line5\": {\n          \"type\": \"string\",\n          \"description\": \"Fifth line of the street address.\",\n          \"maxLength\": 500\n        },\n        \"City\": {\n          \"type\": \"string\",\n          \"description\": \"City name.\",\n          \"\
  maxLength\": 255\n        },\n        \"CountrySubDivisionCode\": {\n          \"type\": \"string\",\n          \"description\": \"Region within a country (e.g., state, province).\",\n          \"maxLength\": 255\n        },\n        \"PostalCode\": {\n          \"type\": \"string\",\n          \"description\": \"Postal code.\",\n          \"maxLength\": 30\n        },\n        \"Country\": {\n          \"type\": \"string\",\n          \"description\": \"Country name or code.\",\n          \"maxLength\": 255\n        },\n        \"Lat\": {\n          \"type\": \"string\",\n          \"description\": \"Latitude coordinate.\"\n        },\n        \"Long\": {\n          \"type\": \"string\",\n          \"description\": \"Longitude coordinate.\"\n        }\n      }\n    },\n    \"EmailAddress\": {\n      \"type\": \"object\",\n      \"description\": \"An email address.\",\n      \"properties\": {\n        \"Address\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n \
  \         \"description\": \"The email address.\",\n          \"maxLength\": 100\n        }\n      }\n    },\n    \"MetaData\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata about entity creation and modification timestamps.\",\n      \"properties\": {\n        \"CreateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp when the entity was created.\"\n        },\n        \"LastUpdatedTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp when the entity was last updated.\"\n        }\n      }\n    },\n    \"LinkedTxn\": {\n      \"type\": \"object\",\n      \"description\": \"A reference to a linked transaction.\",\n      \"properties\": {\n        \"TxnId\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the linked transaction.\"\n        },\n        \"TxnType\": {\n          \"type\": \"string\",\n     \
  \     \"description\": \"The type of the linked transaction.\",\n          \"enum\": [\n            \"Invoice\",\n            \"Payment\",\n            \"CreditMemo\",\n            \"Estimate\",\n            \"SalesReceipt\",\n            \"JournalEntry\",\n            \"Expense\",\n            \"StatementCharge\",\n            \"ReimburseCharge\"\n          ]\n        }\n      },\n      \"required\": [\"TxnId\", \"TxnType\"]\n    },\n    \"SalesItemLineDetail\": {\n      \"type\": \"object\",\n      \"description\": \"Detail for a line item representing a sale of a product or service.\",\n      \"properties\": {\n        \"ItemRef\": {\n          \"$ref\": \"#/$defs/ReferenceType\",\n          \"description\": \"Reference to the item (product or service) being sold.\"\n        },\n        \"ClassRef\": {\n          \"$ref\": \"#/$defs/ReferenceType\",\n          \"description\": \"Reference to the class for classification.\"\n        },\n        \"UnitPrice\": {\n          \"type\": \"\
  number\",\n          \"description\": \"Per-unit selling price of the item.\"\n        },\n        \"RatePercent\": {\n          \"type\": \"number\",\n          \"description\": \"Discount rate as a percentage (for discount lines).\"\n        },\n        \"Qty\": {\n          \"type\": \"number\",\n          \"description\": \"Quantity of items.\"\n        },\n        \"ItemAccountRef\": {\n          \"$ref\": \"#/$defs/ReferenceType\",\n          \"description\": \"Reference to the account associated with this item.\"\n        },\n        \"TaxCodeRef\": {\n          \"$ref\": \"#/$defs/ReferenceType\",\n          \"description\": \"Reference to the tax code for this line.\"\n        },\n        \"ServiceDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Date the service was performed or goods delivered.\"\n        },\n        \"DiscountAmt\": {\n          \"type\": \"number\",\n          \"description\": \"Discount amount applied\
  \ to this line.\"\n        },\n        \"DiscountRate\": {\n          \"type\": \"number\",\n          \"description\": \"Discount rate as a percentage.\"\n        }\n      }\n    },\n    \"InvoiceLine\": {\n      \"type\": \"object\",\n      \"description\": \"A single line item on an invoice.\",\n      \"properties\": {\n        \"Id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the line item.\"\n        },\n        \"LineNum\": {\n          \"type\": \"integer\",\n          \"description\": \"Specifies the position of the line in the collection.\"\n        },\n        \"Description\": {\n          \"type\": \"string\",\n          \"description\": \"Free-form text description of the line item.\",\n          \"maxLength\": 4000\n        },\n        \"Amount\": {\n          \"type\": \"number\",\n          \"description\": \"The total amount for this line item.\"\n        },\n        \"DetailType\": {\n          \"type\": \"string\",\n      \
  \    \"description\": \"The type of detail for this line.\",\n          \"enum\": [\n            \"SalesItemLineDetail\",\n            \"GroupLineDetail\",\n            \"DescriptionOnly\",\n            \"DiscountLineDetail\",\n            \"SubTotalLineDetail\"\n          ]\n        },\n        \"SalesItemLineDetail\": {\n          \"$ref\": \"#/$defs/SalesItemLineDetail\"\n        },\n        \"LinkedTxn\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/LinkedTxn\"\n          }\n        }\n      },\n      \"required\": [\"Amount\", \"DetailType\"]\n    },\n    \"TxnTaxDetail\": {\n      \"type\": \"object\",\n      \"description\": \"Tax details for the transaction.\",\n      \"properties\": {\n        \"TxnTaxCodeRef\": {\n          \"$ref\": \"#/$defs/ReferenceType\",\n          \"description\": \"Reference to the tax code for the transaction.\"\n        },\n        \"TotalTax\": {\n          \"type\": \"number\",\n          \"description\"\
  : \"Total tax calculated for the transaction.\"\n        },\n        \"TaxLine\": {\n          \"type\": \"array\",\n          \"description\": \"Tax lines itemizing individual tax amounts.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"Amount\": {\n                \"type\": \"number\",\n                \"description\": \"Tax amount for this tax line.\"\n              },\n              \"DetailType\": {\n                \"type\": \"string\",\n                \"enum\": [\"TaxLineDetail\"]\n              },\n              \"TaxLineDetail\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"TaxRateRef\": {\n                    \"$ref\": \"#/$defs/ReferenceType\"\n                  },\n                  \"PercentBased\": {\n                    \"type\": \"boolean\"\n                  },\n                  \"TaxPercent\": {\n                    \"type\": \"number\"\n               \
  \   },\n                  \"NetAmountTaxable\": {\n                    \"type\": \"number\"\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"CustomField\": {\n      \"type\": \"object\",\n      \"description\": \"A custom field defined for the entity.\",\n      \"properties\": {\n        \"DefinitionId\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier of the custom field definition.\"\n        },\n        \"Name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the custom field.\"\n        },\n        \"Type\": {\n          \"type\": \"string\",\n          \"description\": \"Data type of the custom field.\",\n          \"enum\": [\"StringType\", \"BooleanType\", \"NumberType\", \"DateType\"]\n        },\n        \"StringValue\": {\n          \"type\": \"string\",\n          \"description\": \"Value when Type is StringType.\"\n        }\n      }\n    }\n \
  \ },\n  \"examples\": [\n    {\n      \"CustomerRef\": {\n        \"value\": \"1\",\n        \"name\": \"Amy's Bird Sanctuary\"\n      },\n      \"Line\": [\n        {\n          \"Amount\": 150.00,\n          \"DetailType\": \"SalesItemLineDetail\",\n          \"SalesItemLineDetail\": {\n            \"ItemRef\": {\n              \"value\": \"1\",\n              \"name\": \"Services\"\n            },\n            \"UnitPrice\": 150,\n            \"Qty\": 1\n          }\n        },\n        {\n          \"Amount\": 150.00,\n          \"DetailType\": \"SubTotalLineDetail\"\n        }\n      ],\n      \"DueDate\": \"2025-12-15\",\n      \"TxnDate\": \"2025-11-15\",\n      \"DocNumber\": \"1001\",\n      \"BillEmail\": {\n        \"Address\": \"amy@birdsnest.example.com\"\n      }\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/intuit/refs/heads/main/json-schema/intuit-invoice-schema.json
tags:
- Accounting
- Custom Fields
- Financial
- Financial Services
- Invoicing
- Payments
- Payroll
- Project Management
- Sales Tax
- Small Business
- Tax
- Tax Preparation
- Taxes
- Time Tracking
title: QuickBooks Online Invoice
---
