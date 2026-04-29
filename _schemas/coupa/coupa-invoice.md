---
description: Schema representing a Coupa invoice, which is a billing document from a supplier for goods or services delivered. Supports the full invoice lifecycle from draft through approval, dispute, and payment. Based on the Coupa Core API invoices resource as documented at compass.coupa.com.
layout: schema
name: Coupa Invoice
properties_list:
- description: Coupa unique internal identifier for the invoice.
  name: id
  type: integer
- description: Invoice identification number assigned by the supplier.
  name: invoice-number
  type: string
- description: Date of the invoice. Provide only the date (not timestamp) to prevent credit note issues.
  name: invoice-date
  type: string
- description: Current status of the invoice in its lifecycle.
  name: status
  type: string
- description: Document type classification.
  name: document-type
  type: string
- description: The supplier (vendor) who issued this invoice.
  name: supplier
  type: object
- description: Transaction currency for the invoice.
  name: currency
  type: object
- description: Total invoice amount including tax.
  name: gross-total
  type:
  - number
  - 'null'
- description: Header-level tax amount. Not used if tax is provided at the line level.
  name: tax-amount
  type:
  - number
  - 'null'
- description: Header-level tax classification code.
  name: tax-code
  type:
  - string
  - 'null'
- description: Header-level tax rate percentage.
  name: tax-rate
  type:
  - number
  - 'null'
- description: Flag indicating whether taxes are provided at the line level rather than the header level.
  name: line-level-taxation
  type: boolean
- description: Discount amount provided by the supplier.
  name: discount-amount
  type:
  - number
  - 'null'
- description: Discount percentage.
  name: discount-percent
  type:
  - number
  - 'null'
- description: Date by which payment must be made to qualify for the discount.
  name: discount-due-date
  type:
  - string
  - 'null'
- description: Amount due less discount.
  name: discount-due-less-discount
  type:
  - number
  - 'null'
- description: Total amount due after discount application.
  name: amount-due-less-discount
  type:
  - number
  - 'null'
- description: Gross total minus the discount amount.
  name: gross-total-less-discount
  type:
  - number
  - 'null'
- description: Net total minus the discount amount.
  name: net-total-less-discount
  type:
  - number
  - 'null'
- description: Freight charges on the invoice.
  name: shipping-amount
  type:
  - number
  - 'null'
- description: Processing and handling fees.
  name: handling-amount
  type:
  - number
  - 'null'
- description: Payment schedule terms for the invoice.
  name: payment-term
  type: object
- description: Payment processing method.
  name: payment-method
  type:
  - string
  - 'null'
- description: Payment-related notes.
  name: payment-notes
  type:
  - string
  - 'null'
- description: Actual payment date.
  name: payment-date
  type:
  - string
  - 'null'
- description: Payment order reference number.
  name: payment-order-reference
  type:
  - string
  - 'null'
- description: Net payment due date.
  name: net-due-date
  type:
  - string
  - 'null'
- description: Currency exchange rate (up to 9 decimal places).
  name: exchange-rate
  type:
  - number
  - 'null'
- description: Billing address for the invoice.
  name: bill-to-address
  type: object
- description: Shipping destination address.
  name: ship-to-address
  type: object
- description: Supplier ship-from address.
  name: ship-from-address
  type:
  - object
  - 'null'
- description: Vendor address on the invoice.
  name: invoice-from-address
  type:
  - object
  - 'null'
- description: Remit-to address for payment.
  name: remit-to-address
  type: object
- description: Supplier remit-to address reference.
  name: supplier-remit-to
  type:
  - object
  - 'null'
- description: Collection of invoice line items.
  name: invoice-lines
  type: array
- description: Collection of invoice charge allocations.
  name: invoice-charges
  type: array
- description: Tax line details for line-level taxation.
  name: tax-lines
  type: array
- description: Withholding tax line details.
  name: withholding-tax-lines
  type: array
- description: Withholding tax override amount.
  name: withholding-tax-override
  type:
  - number
  - 'null'
- description: Indicates whether this document is a credit note.
  name: is-credit-note
  type: boolean
- description: Original invoice number. Required when is-credit-note is true.
  name: original-invoice-number
  type:
  - string
  - 'null'
- description: Original invoice date. Required when is-credit-note is true. Provide only the date.
  name: original-invoice-date
  type:
  - string
  - 'null'
- description: Reason for the credit adjustment.
  name: credit-reason
  type:
  - string
  - 'null'
- description: Variance amount between the credit note and the original invoice.
  name: credit-note-differences-with-original-invoice
  type:
  - number
  - 'null'
- description: Invoice comments.
  name: comments
  type:
  - string
  - 'null'
- description: Internal note (not visible to supplier).
  name: internal-note
  type:
  - string
  - 'null'
- description: Note from the supplier.
  name: supplier-note
  type:
  - string
  - 'null'
- description: Invoice confirmation status.
  name: confirmation
  type:
  - string
  - 'null'
- description: Associated contract reference.
  name: contract
  type:
  - object
  - 'null'
- description: User who requested the invoice.
  name: requested-by
  type: object
- description: Whether the invoice has been paid.
  name: paid
  type: boolean
- description: Whether the invoice passes compliance validation.
  name: compliant
  type: boolean
- description: Whether the invoice has been cancelled.
  name: canceled
  type: boolean
- description: Whether the invoice was created by the supplier via CSP.
  name: supplier-created
  type: boolean
- description: Whether the invoice has been exported to an external system (e.g., ERP).
  name: exported
  type: boolean
- description: Delivery date for the goods or services.
  name: delivery-date
  type:
  - string
  - 'null'
- description: Purchaser tax registration. Required for compliant invoicing.
  name: buyer-tax-registration
  type:
  - object
  - 'null'
- description: Supplier tax registration. Required for compliant invoicing.
  name: supplier-tax-registration
  type:
  - object
  - 'null'
- description: Legal destination country for compliance purposes.
  name: legal-destination-country
  type:
  - object
  - 'null'
- description: Destination country for compliance.
  name: destination-country
  type:
  - object
  - 'null'
- description: Country of origin for the goods.
  name: origin-country
  type:
  - object
  - 'null'
- description: Gross total in the origin country currency.
  name: origin-currency-gross
  type:
  - number
  - 'null'
- description: Net total in the origin country currency.
  name: origin-currency-net
  type:
  - number
  - 'null'
- description: Tax amount in the origin country currency.
  name: taxes-in-origin-country-currency
  type:
  - number
  - 'null'
- description: Cash accounting scheme reference flag.
  name: cash-accounting-scheme-reference
  type:
  - string
  - 'null'
- description: Margin scheme reason.
  name: margin-scheme
  type:
  - string
  - 'null'
- description: Reverse charge reference information.
  name: reverse-charge-reference
  type:
  - string
  - 'null'
- description: Invoice image scan identifier.
  name: image-scan
  type:
  - string
  - 'null'
- description: URL of the scanned invoice image.
  name: image-scan-url
  type:
  - string
  - 'null'
- description: File name of the scanned image.
  name: image-scan-file-name
  type:
  - string
  - 'null'
- description: File size of the scanned image.
  name: image-scan-file-size
  type:
  - string
  - 'null'
- description: MIME content type of the scanned image.
  name: image-scan-content-type
  type:
  - string
  - 'null'
- description: Approval workflow records associated with this invoice.
  name: approvals
  type: array
- description: Reason insight for abandoning the invoice.
  name: abandon-reason
  type:
  - object
  - 'null'
- description: Reasons for disputing the invoice.
  name: dispute-reasons
  type: array
- description: Method used to dispute the invoice.
  name: dispute-method
  type:
  - string
  - 'null'
- description: Description of tolerance check failures.
  name: tolerance-failures
  type:
  - string
  - 'null'
- description: Payment records associated with this invoice.
  name: payments
  type: array
- description: File attachments linked to the invoice.
  name: attachments
  type: array
- description: Tags associated with the invoice.
  name: tags
  type: array
- description: Tag association records.
  name: taggings
  type: array
- description: Timestamp when the invoice was created. Automatically set by Coupa.
  name: created-at
  type: string
- description: Timestamp when the invoice was last updated. Automatically set by Coupa.
  name: updated-at
  type: string
- description: The user who created the invoice.
  name: created-by
  type: object
- description: The user who last updated the invoice.
  name: updated-by
  type: object
provider_name: Coupa
provider_slug: coupa
schema_file: json-schema/coupa-invoice-schema.json
slug: coupa-invoice
source_filename: coupa-invoice-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/coupa/json-schema/coupa-invoice-schema.json\",\n  \"title\": \"Coupa Invoice\",\n  \"description\": \"Schema representing a Coupa invoice, which is a billing document from a supplier for goods or services delivered. Supports the full invoice lifecycle from draft through approval, dispute, and payment. Based on the Coupa Core API invoices resource as documented at compass.coupa.com.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Coupa unique internal identifier for the invoice.\",\n      \"readOnly\": true\n    },\n    \"invoice-number\": {\n      \"type\": \"string\",\n      \"description\": \"Invoice identification number assigned by the supplier.\",\n      \"maxLength\": 40\n    },\n    \"invoice-date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"\
  Date of the invoice. Provide only the date (not timestamp) to prevent credit note issues.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the invoice in its lifecycle.\",\n      \"enum\": [\n        \"new\",\n        \"draft\",\n        \"pending_approval\",\n        \"approved\",\n        \"pending_receipt\",\n        \"processing\",\n        \"payable_adjustment\",\n        \"on_hold\",\n        \"ap_hold\",\n        \"booking_hold\",\n        \"pending_action\",\n        \"rejected\",\n        \"disputed\",\n        \"abandoned\",\n        \"voided\",\n        \"invalid\"\n      ]\n    },\n    \"document-type\": {\n      \"type\": \"string\",\n      \"description\": \"Document type classification.\",\n      \"enum\": [\n        \"Invoice\",\n        \"Credit Note\"\n      ]\n    },\n    \"supplier\": {\n      \"$ref\": \"#/$defs/SupplierReference\",\n      \"description\": \"The supplier (vendor) who issued this invoice.\"\n    },\n\
  \    \"currency\": {\n      \"$ref\": \"#/$defs/CurrencyReference\",\n      \"description\": \"Transaction currency for the invoice.\"\n    },\n    \"gross-total\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Total invoice amount including tax.\",\n      \"multipleOf\": 0.0001\n    },\n    \"tax-amount\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Header-level tax amount. Not used if tax is provided at the line level.\",\n      \"multipleOf\": 0.0001\n    },\n    \"tax-code\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Header-level tax classification code.\",\n      \"maxLength\": 255\n    },\n    \"tax-rate\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Header-level tax rate percentage.\"\n    },\n    \"line-level-taxation\": {\n      \"type\": \"boolean\",\n      \"description\": \"Flag indicating whether taxes are provided at the line level rather than the header level.\"\n    },\n\
  \    \"discount-amount\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Discount amount provided by the supplier.\",\n      \"multipleOf\": 0.0001\n    },\n    \"discount-percent\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Discount percentage.\"\n    },\n    \"discount-due-date\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"Date by which payment must be made to qualify for the discount.\"\n    },\n    \"discount-due-less-discount\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Amount due less discount.\",\n      \"readOnly\": true\n    },\n    \"amount-due-less-discount\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Total amount due after discount application.\",\n      \"readOnly\": true\n    },\n    \"gross-total-less-discount\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Gross total minus the discount amount.\"\
  ,\n      \"readOnly\": true\n    },\n    \"net-total-less-discount\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Net total minus the discount amount.\",\n      \"readOnly\": true\n    },\n    \"shipping-amount\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Freight charges on the invoice.\",\n      \"multipleOf\": 0.0001\n    },\n    \"handling-amount\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Processing and handling fees.\",\n      \"multipleOf\": 0.0001\n    },\n    \"payment-term\": {\n      \"$ref\": \"#/$defs/PaymentTermReference\",\n      \"description\": \"Payment schedule terms for the invoice.\"\n    },\n    \"payment-method\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Payment processing method.\",\n      \"maxLength\": 10\n    },\n    \"payment-notes\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Payment-related notes.\"\n    },\n    \"payment-date\"\
  : {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"Actual payment date.\"\n    },\n    \"payment-order-reference\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Payment order reference number.\",\n      \"maxLength\": 255\n    },\n    \"net-due-date\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"Net payment due date.\"\n    },\n    \"exchange-rate\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Currency exchange rate (up to 9 decimal places).\",\n      \"multipleOf\": 0.000000001\n    },\n    \"bill-to-address\": {\n      \"$ref\": \"#/$defs/AddressReference\",\n      \"description\": \"Billing address for the invoice.\"\n    },\n    \"ship-to-address\": {\n      \"$ref\": \"#/$defs/AddressReference\",\n      \"description\": \"Shipping destination address.\"\n    },\n    \"ship-from-address\": {\n      \"type\": [\"object\", \"null\"],\n\
  \      \"description\": \"Supplier ship-from address.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"invoice-from-address\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Vendor address on the invoice.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"remit-to-address\": {\n      \"$ref\": \"#/$defs/AddressReference\",\n      \"description\": \"Remit-to address for payment.\"\n    },\n    \"supplier-remit-to\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Supplier remit-to address reference.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"invoice-lines\": {\n      \"type\": \"array\",\n      \"description\": \"Collection\
  \ of invoice line items.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/InvoiceLine\"\n      }\n    },\n    \"invoice-charges\": {\n      \"type\": \"array\",\n      \"description\": \"Collection of invoice charge allocations.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/InvoiceCharge\"\n      }\n    },\n    \"tax-lines\": {\n      \"type\": \"array\",\n      \"description\": \"Tax line details for line-level taxation.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/TaxLine\"\n      }\n    },\n    \"withholding-tax-lines\": {\n      \"type\": \"array\",\n      \"description\": \"Withholding tax line details.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/WithholdingTaxLine\"\n      }\n    },\n    \"withholding-tax-override\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Withholding tax override amount.\",\n      \"multipleOf\": 0.001\n    },\n    \"is-credit-note\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether\
  \ this document is a credit note.\"\n    },\n    \"original-invoice-number\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Original invoice number. Required when is-credit-note is true.\",\n      \"maxLength\": 40\n    },\n    \"original-invoice-date\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"Original invoice date. Required when is-credit-note is true. Provide only the date.\"\n    },\n    \"credit-reason\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Reason for the credit adjustment.\",\n      \"maxLength\": 255\n    },\n    \"credit-note-differences-with-original-invoice\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Variance amount between the credit note and the original invoice.\",\n      \"multipleOf\": 0.0001\n    },\n    \"comments\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Invoice comments.\",\n      \"maxLength\": 255\n\
  \    },\n    \"internal-note\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Internal note (not visible to supplier).\"\n    },\n    \"supplier-note\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Note from the supplier.\"\n    },\n    \"confirmation\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Invoice confirmation status.\",\n      \"maxLength\": 50\n    },\n    \"contract\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Associated contract reference.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"requested-by\": {\n      \"$ref\": \"#/$defs/UserReference\",\n      \"description\": \"User who requested the invoice.\"\n    },\n    \"paid\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the invoice has been paid.\",\n      \"readOnly\": true\n\
  \    },\n    \"compliant\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the invoice passes compliance validation.\",\n      \"readOnly\": true\n    },\n    \"canceled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the invoice has been cancelled.\",\n      \"readOnly\": true\n    },\n    \"supplier-created\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the invoice was created by the supplier via CSP.\",\n      \"readOnly\": true\n    },\n    \"exported\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the invoice has been exported to an external system (e.g., ERP).\"\n    },\n    \"delivery-date\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"Delivery date for the goods or services.\"\n    },\n    \"buyer-tax-registration\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Purchaser tax registration. Required for compliant invoicing.\"\
  ,\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\"\n        },\n        \"number\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"supplier-tax-registration\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Supplier tax registration. Required for compliant invoicing.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\"\n        },\n        \"number\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"legal-destination-country\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Legal destination country for compliance purposes.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\"\n        },\n        \"code\": {\n          \"type\": \"string\",\n          \"description\": \"ISO 3166-1 alpha-2 country code.\"\n        }\n      }\n    },\n    \"destination-country\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\"\
  : \"Destination country for compliance.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\"\n        },\n        \"code\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"origin-country\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Country of origin for the goods.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\"\n        },\n        \"code\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"origin-currency-gross\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Gross total in the origin country currency.\",\n      \"multipleOf\": 0.0001\n    },\n    \"origin-currency-net\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Net total in the origin country currency.\",\n      \"multipleOf\": 0.0001\n    },\n    \"taxes-in-origin-country-currency\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Tax amount\
  \ in the origin country currency.\",\n      \"multipleOf\": 0.0001\n    },\n    \"cash-accounting-scheme-reference\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Cash accounting scheme reference flag.\",\n      \"maxLength\": 255\n    },\n    \"margin-scheme\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Margin scheme reason.\",\n      \"maxLength\": 255\n    },\n    \"reverse-charge-reference\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Reverse charge reference information.\",\n      \"maxLength\": 255\n    },\n    \"image-scan\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Invoice image scan identifier.\",\n      \"maxLength\": 25\n    },\n    \"image-scan-url\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"URL of the scanned invoice image.\",\n      \"maxLength\": 255\n    },\n    \"image-scan-file-name\": {\n      \"type\": [\"string\"\
  , \"null\"],\n      \"description\": \"File name of the scanned image.\",\n      \"maxLength\": 255\n    },\n    \"image-scan-file-size\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"File size of the scanned image.\",\n      \"maxLength\": 12\n    },\n    \"image-scan-content-type\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"MIME content type of the scanned image.\",\n      \"maxLength\": 191\n    },\n    \"approvals\": {\n      \"type\": \"array\",\n      \"description\": \"Approval workflow records associated with this invoice.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ApprovalReference\"\n      },\n      \"readOnly\": true\n    },\n    \"abandon-reason\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Reason insight for abandoning the invoice.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\"\n        },\n        \"description\": {\n          \"type\": \"string\"\n     \
  \   }\n      }\n    },\n    \"dispute-reasons\": {\n      \"type\": \"array\",\n      \"description\": \"Reasons for disputing the invoice.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"integer\"\n          },\n          \"description\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"dispute-method\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Method used to dispute the invoice.\",\n      \"maxLength\": 10\n    },\n    \"tolerance-failures\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Description of tolerance check failures.\",\n      \"maxLength\": 512\n    },\n    \"payments\": {\n      \"type\": \"array\",\n      \"description\": \"Payment records associated with this invoice.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"integer\"\n  \
  \        },\n          \"amount\": {\n            \"type\": \"number\"\n          },\n          \"payment-date\": {\n            \"type\": \"string\",\n            \"format\": \"date\"\n          }\n        }\n      },\n      \"readOnly\": true\n    },\n    \"attachments\": {\n      \"type\": \"array\",\n      \"description\": \"File attachments linked to the invoice.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/AttachmentReference\"\n      }\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags associated with the invoice.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"integer\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"taggings\": {\n      \"type\": \"array\",\n      \"description\": \"Tag association records.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n \
  \         \"id\": {\n            \"type\": \"integer\"\n          }\n        }\n      }\n    },\n    \"created-at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the invoice was created. Automatically set by Coupa.\",\n      \"readOnly\": true\n    },\n    \"updated-at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the invoice was last updated. Automatically set by Coupa.\",\n      \"readOnly\": true\n    },\n    \"created-by\": {\n      \"$ref\": \"#/$defs/UserReference\",\n      \"description\": \"The user who created the invoice.\"\n    },\n    \"updated-by\": {\n      \"$ref\": \"#/$defs/UserReference\",\n      \"description\": \"The user who last updated the invoice.\"\n    }\n  },\n  \"required\": [\n    \"invoice-number\",\n    \"invoice-date\",\n    \"supplier\",\n    \"currency\",\n    \"invoice-lines\"\n  ],\n  \"$defs\": {\n    \"UserReference\": {\n   \
  \   \"type\": \"object\",\n      \"description\": \"Reference to a Coupa user.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Coupa unique identifier for the user.\"\n        },\n        \"login\": {\n          \"type\": \"string\",\n          \"description\": \"User login name.\"\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"User email address.\"\n        }\n      }\n    },\n    \"SupplierReference\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to a supplier (vendor) in Coupa.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Coupa unique identifier for the supplier.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Supplier name.\",\n          \"maxLength\": 100\n        },\n        \"number\": {\n         \
  \ \"type\": \"string\",\n          \"description\": \"Supplier number.\"\n        }\n      }\n    },\n    \"CurrencyReference\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to a currency.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Coupa unique identifier for the currency.\"\n        },\n        \"code\": {\n          \"type\": \"string\",\n          \"description\": \"ISO 4217 currency code.\",\n          \"pattern\": \"^[A-Z]{3}$\",\n          \"examples\": [\"USD\", \"EUR\", \"GBP\"]\n        }\n      }\n    },\n    \"AddressReference\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to a physical address in Coupa.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Coupa unique identifier for the address.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Address name or\
  \ label.\"\n        },\n        \"street1\": {\n          \"type\": \"string\",\n          \"description\": \"Street address line 1.\"\n        },\n        \"street2\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Street address line 2.\"\n        },\n        \"city\": {\n          \"type\": \"string\",\n          \"description\": \"City name.\"\n        },\n        \"state\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"State or province.\"\n        },\n        \"postal-code\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Postal or ZIP code.\"\n        },\n        \"country\": {\n          \"type\": \"object\",\n          \"description\": \"Country reference.\",\n          \"properties\": {\n            \"id\": {\n              \"type\": \"integer\"\n            },\n            \"code\": {\n              \"type\": \"string\",\n              \"description\": \"ISO 3166-1 alpha-2 country code.\"\
  \n            }\n          }\n        }\n      }\n    },\n    \"PaymentTermReference\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to a payment term definition.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Coupa unique identifier for the payment term.\"\n        },\n        \"code\": {\n          \"type\": \"string\",\n          \"description\": \"Payment term code.\"\n        }\n      }\n    },\n    \"InvoiceLine\": {\n      \"type\": \"object\",\n      \"description\": \"A line item on an invoice representing a specific good or service being billed.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Coupa unique identifier for the invoice line.\",\n          \"readOnly\": true\n        },\n        \"line-num\": {\n          \"type\": \"integer\",\n          \"description\": \"Sequential line number.\"\n        },\n        \"description\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"Description of the item or service.\",\n          \"maxLength\": 255\n        },\n        \"quantity\": {\n          \"type\": \"number\",\n          \"description\": \"Quantity invoiced.\"\n        },\n        \"price\": {\n          \"type\": \"number\",\n          \"description\": \"Unit price of the item.\"\n        },\n        \"total\": {\n          \"type\": \"number\",\n          \"description\": \"Line total (quantity multiplied by price).\",\n          \"readOnly\": true\n        },\n        \"uom\": {\n          \"type\": \"object\",\n          \"description\": \"Unit of measure.\",\n          \"properties\": {\n            \"id\": {\n              \"type\": \"integer\"\n            },\n            \"code\": {\n              \"type\": \"string\",\n              \"description\": \"Unit of measure code (e.g., EA, CS, BX).\"\n            }\n          }\n        },\n        \"tax-amount\": {\n          \"type\":\
  \ [\"number\", \"null\"],\n          \"description\": \"Tax amount for this line.\"\n        },\n        \"tax-code\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Tax classification code for this line.\"\n        },\n        \"tax-rate\": {\n          \"type\": [\"number\", \"null\"],\n          \"description\": \"Tax rate percentage for this line.\"\n        },\n        \"order-line-id\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"Reference to the backing purchase order line.\"\n        },\n        \"commodity\": {\n          \"type\": [\"object\", \"null\"],\n          \"description\": \"Commodity classification for the line item.\",\n          \"properties\": {\n            \"id\": {\n              \"type\": \"integer\"\n            },\n            \"name\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"account\": {\n          \"type\": [\"object\", \"null\"],\n          \"\
  description\": \"Chart of accounts reference for cost allocation.\",\n          \"properties\": {\n            \"id\": {\n              \"type\": \"integer\"\n            },\n            \"code\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"currency\": {\n          \"$ref\": \"#/$defs/CurrencyReference\"\n        },\n        \"created-at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp when the line was created.\",\n          \"readOnly\": true\n        },\n        \"updated-at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp when the line was last updated.\",\n          \"readOnly\": true\n        }\n      },\n      \"required\": [\n        \"description\",\n        \"quantity\",\n        \"price\"\n      ]\n    },\n    \"InvoiceCharge\": {\n      \"type\": \"object\",\n      \"description\": \"A charge allocation\
  \ on an invoice (e.g., shipping, handling, miscellaneous).\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Coupa unique identifier for the charge.\",\n          \"readOnly\": true\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Charge type (e.g., ShippingCharge, HandlingCharge, MiscCharge).\"\n        },\n        \"amount\": {\n          \"type\": \"number\",\n          \"description\": \"Charge amount.\"\n        },\n        \"account\": {\n          \"type\": [\"object\", \"null\"],\n          \"properties\": {\n            \"id\": {\n              \"type\": \"integer\"\n            },\n            \"code\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    },\n    \"TaxLine\": {\n      \"type\": \"object\",\n      \"description\": \"Tax line detail for line-level taxation.\",\n      \"properties\": {\n        \"id\": {\n          \"\
  type\": \"integer\",\n          \"readOnly\": true\n        },\n        \"amount\": {\n          \"type\": \"number\",\n          \"description\": \"Tax amount.\"\n        },\n        \"rate\": {\n          \"type\": \"number\",\n          \"description\": \"Tax rate percentage.\"\n        },\n        \"code\": {\n          \"type\": \"string\",\n          \"description\": \"Tax code.\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Tax line description.\"\n        }\n      }\n    },\n    \"WithholdingTaxLine\": {\n      \"type\": \"object\",\n      \"description\": \"Withholding tax line detail.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"readOnly\": true\n        },\n        \"amount\": {\n          \"type\": \"number\",\n          \"description\": \"Withholding tax amount.\"\n        },\n        \"rate\": {\n          \"type\": \"number\",\n          \"description\": \"Withholding\
  \ tax rate percentage.\"\n        },\n        \"code\": {\n          \"type\": \"string\",\n          \"description\": \"Withholding tax code.\"\n        }\n      }\n    },\n    \"ApprovalReference\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to an approval record.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Coupa unique identifier for the approval.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Approval status.\"\n        },\n        \"approver\": {\n          \"$ref\": \"#/$defs/UserReference\",\n          \"description\": \"User assigned as approver.\"\n        },\n        \"approval-date\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date-time\",\n          \"description\": \"When the approval was granted.\"\n        }\n      }\n    },\n    \"AttachmentReference\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"Reference to a file attachment.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Coupa unique identifier for the attachment.\"\n        },\n        \"file-name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the attached file.\"\n        },\n        \"file-url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to download the attachment.\"\n        }\n      }\n    }\n  },\n  \"examples\": [\n    {\n      \"id\": 1,\n      \"invoice-number\": \"INV-2024-001\",\n      \"invoice-date\": \"2024-03-15\",\n      \"status\": \"pending_approval\",\n      \"document-type\": \"Invoice\",\n      \"supplier\": {\n        \"id\": 42,\n        \"name\": \"Acme Office Supplies\",\n        \"number\": \"SUP-001\"\n      },\n      \"currency\": {\n        \"id\": 1,\n        \"code\": \"USD\"\n      },\n      \"gross-total\": 5250.00,\n      \"tax-amount\":\
  \ 250.00,\n      \"line-level-taxation\": false,\n      \"payment-term\": {\n        \"id\": 1,\n        \"code\": \"Net 30\"\n      },\n      \"bill-to-address\": {\n        \"id\": 5,\n        \"name\": \"Main Office\",\n        \"street1\": \"123 Business Ave\",\n        \"city\": \"San Francisco\",\n        \"state\": \"CA\",\n        \"postal-code\": \"94105\",\n        \"country\": {\n          \"id\": 1,\n          \"code\": \"US\"\n        }\n      },\n      \"invoice-lines\": [\n        {\n          \"id\": 101,\n          \"line-num\": 1,\n          \"description\": \"Office Desk Chair - Ergonomic\",\n          \"quantity\": 10,\n          \"price\": 500.00,\n          \"total\": 5000.00,\n          \"uom\": {\n            \"id\": 1,\n            \"code\": \"EA\"\n          },\n          \"order-line-id\": 201\n        }\n      ],\n      \"is-credit-note\": false,\n      \"exported\": false,\n      \"paid\": false,\n      \"compliant\": true,\n      \"created-at\": \"2024-03-15T10:30:00+00:00\"\
  ,\n      \"updated-at\": \"2024-03-15T10:30:00+00:00\"\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/coupa/refs/heads/main/json-schema/coupa-invoice-schema.json
tags:
- BSM
- Business Spend Management
- Cloud Platform
- Enterprise
- Financial Management
- Invoicing
- Procurement
- Supply Chain
title: Coupa Invoice
---
