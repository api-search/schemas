---
description: A statement of the money due for goods or services; a bill.
layout: schema
name: Schema.org Invoice
properties_list:
- description: The Schema.org type.
  name: '@type'
  type: string
- description: ''
  name: '@context'
  type: string
- description: The identifier for the account the payment will be applied to.
  name: accountId
  type: string
- description: A number that confirms the given order or payment.
  name: confirmationNumber
  type: string
- description: Party placing the order or paying the invoice.
  name: customer
  type: object
- description: An entity that arranges for an exchange.
  name: broker
  type: object
- description: The service provider.
  name: provider
  type: object
- description: The time interval used to compute the invoice in ISO 8601 format.
  name: billingPeriod
  type: string
- description: The date that payment is due.
  name: paymentDueDate
  type: string
- description: The name of the credit card or other method of payment.
  name: paymentMethod
  type: string
- description: An identifier for the method of payment used.
  name: paymentMethodId
  type: string
- description: The status of payment.
  name: paymentStatus
  type: string
- description: The date the invoice is scheduled to be paid.
  name: scheduledPaymentDate
  type: string
- description: The total amount due.
  name: totalPaymentDue
  type: object
- description: The minimum payment required at this time.
  name: minimumPaymentDue
  type: object
- description: The Order(s) related to this Invoice.
  name: referencesOrder
  type: object
- description: A category for the invoice.
  name: category
  type: string
- description: URL of the invoice.
  name: url
  type: string
provider_name: Schema.org
provider_slug: schema-org
schema_file: json-schema/schema-org-invoice-schema.json
slug: schema-org-invoice
source_filename: schema-org-invoice-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.org/schemas/invoice.json\",\n  \"title\": \"Schema.org Invoice\",\n  \"description\": \"A statement of the money due for goods or services; a bill.\",\n  \"type\": \"object\",\n  \"required\": [\"@type\"],\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"const\": \"Invoice\",\n      \"description\": \"The Schema.org type.\"\n    },\n    \"@context\": {\n      \"type\": \"string\",\n      \"default\": \"https://schema.org\"\n    },\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier for the account the payment will be applied to.\"\n    },\n    \"confirmationNumber\": {\n      \"type\": \"string\",\n      \"description\": \"A number that confirms the given order or payment.\"\n    },\n    \"customer\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-person-schema.json\" },\n        { \"$ref\": \"schema-org-organization-schema.json\"\
  \ }\n      ],\n      \"description\": \"Party placing the order or paying the invoice.\"\n    },\n    \"broker\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-person-schema.json\" },\n        { \"$ref\": \"schema-org-organization-schema.json\" }\n      ],\n      \"description\": \"An entity that arranges for an exchange.\"\n    },\n    \"provider\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-person-schema.json\" },\n        { \"$ref\": \"schema-org-organization-schema.json\" }\n      ],\n      \"description\": \"The service provider.\"\n    },\n    \"billingPeriod\": {\n      \"type\": \"string\",\n      \"description\": \"The time interval used to compute the invoice in ISO 8601 format.\"\n    },\n    \"paymentDueDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date that payment is due.\"\n    },\n    \"paymentMethod\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the credit card or other\
  \ method of payment.\"\n    },\n    \"paymentMethodId\": {\n      \"type\": \"string\",\n      \"description\": \"An identifier for the method of payment used.\"\n    },\n    \"paymentStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\"PaymentAutomaticallyApplied\", \"PaymentComplete\", \"PaymentDeclined\", \"PaymentDue\", \"PaymentPastDue\"],\n      \"description\": \"The status of payment.\"\n    },\n    \"scheduledPaymentDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The date the invoice is scheduled to be paid.\"\n    },\n    \"totalPaymentDue\": {\n      \"type\": \"object\",\n      \"description\": \"The total amount due.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"MonetaryAmount\" },\n        \"value\": { \"type\": \"number\", \"description\": \"The amount.\" },\n        \"currency\": { \"type\": \"string\", \"pattern\": \"^[A-Z]{3}$\", \"description\": \"The currency (ISO 4217).\" }\n\
  \      }\n    },\n    \"minimumPaymentDue\": {\n      \"type\": \"object\",\n      \"description\": \"The minimum payment required at this time.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"MonetaryAmount\" },\n        \"value\": { \"type\": \"number\" },\n        \"currency\": { \"type\": \"string\", \"pattern\": \"^[A-Z]{3}$\" }\n      }\n    },\n    \"referencesOrder\": {\n      \"$ref\": \"schema-org-order-schema.json\",\n      \"description\": \"The Order(s) related to this Invoice.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"A category for the invoice.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the invoice.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-org/refs/heads/main/json-schema/schema-org-invoice-schema.json
tags:
- Schema.org
- Structured Data
- Linked Data
- JSON-LD
- Vocabulary
- SEO
- Web Standards
- RDF
- Ontology
title: Schema.org Invoice
---
