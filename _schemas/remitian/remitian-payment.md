---
description: Schema representing a tax payment processed through the Remitian Tax Payment API, covering the full lifecycle from initiation through validation, confirmation, and completion.
layout: schema
name: Remitian Tax Payment
properties_list:
- description: Unique payment identifier assigned by Remitian
  name: id
  type: string
- description: Current lifecycle status of the payment
  name: status
  type: string
- description: Payment amount in the specified currency
  name: amount
  type: number
- description: Three-letter ISO 4217 currency code
  name: currency
  type: string
- description: Type of tax being paid, as defined by the target jurisdiction
  name: taxType
  type: string
- description: Tax period the payment applies to (e.g., 2025, 2025-Q4, 2025-03)
  name: taxPeriod
  type: string
- description: Identifier of the target tax jurisdiction
  name: jurisdictionId
  type: string
- description: Identifier of the client account making the payment
  name: accountId
  type: string
- description: Taxpayer identification number (EIN, SSN, BN) as required by the jurisdiction
  name: taxIdentifier
  type: string
- description: ''
  name: validationResults
  type: object
- description: Confirmation number issued by the tax authority upon successful processing
  name: confirmationNumber
  type: string
- description: Timestamp when the payment was initiated
  name: createdAt
  type: string
- description: Timestamp of the last status update
  name: updatedAt
  type: string
- description: Arbitrary key-value pairs for partner-specific reference data
  name: metadata
  type: object
provider_name: Remitian
provider_slug: remitian
schema_file: json-schema/remitian-payment-schema.json
slug: remitian-payment
source_filename: remitian-payment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://remitian.com/schemas/remitian/payment.json\",\n  \"title\": \"Remitian Tax Payment\",\n  \"description\": \"Schema representing a tax payment processed through the Remitian Tax Payment API, covering the full lifecycle from initiation through validation, confirmation, and completion.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"id\",\n    \"status\",\n    \"amount\",\n    \"currency\",\n    \"taxType\",\n    \"taxPeriod\",\n    \"jurisdictionId\",\n    \"accountId\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique payment identifier assigned by Remitian\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current lifecycle status of the payment\",\n      \"enum\": [\n        \"draft\",\n        \"validated\",\n        \"confirmed\",\n        \"processing\",\n        \"completed\",\n        \"\
  failed\",\n        \"cancelled\"\n      ]\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"description\": \"Payment amount in the specified currency\",\n      \"minimum\": 0.01\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Three-letter ISO 4217 currency code\",\n      \"pattern\": \"^[A-Z]{3}$\",\n      \"minLength\": 3,\n      \"maxLength\": 3\n    },\n    \"taxType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of tax being paid, as defined by the target jurisdiction\",\n      \"minLength\": 1\n    },\n    \"taxPeriod\": {\n      \"type\": \"string\",\n      \"description\": \"Tax period the payment applies to (e.g., 2025, 2025-Q4, 2025-03)\",\n      \"pattern\": \"^\\\\d{4}(-Q[1-4]|-\\\\d{2})?$\"\n    },\n    \"jurisdictionId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the target tax jurisdiction\"\n    },\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"\
  Identifier of the client account making the payment\"\n    },\n    \"taxIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"Taxpayer identification number (EIN, SSN, BN) as required by the jurisdiction\"\n    },\n    \"validationResults\": {\n      \"$ref\": \"#/$defs/ValidationResult\"\n    },\n    \"confirmationNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Confirmation number issued by the tax authority upon successful processing\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the payment was initiated\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the last status update\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Arbitrary key-value pairs for partner-specific\
  \ reference data\"\n    }\n  },\n  \"$defs\": {\n    \"ValidationResult\": {\n      \"type\": \"object\",\n      \"description\": \"Results of jurisdiction-specific payment validation\",\n      \"properties\": {\n        \"valid\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the payment passed all validation checks\"\n        },\n        \"errors\": {\n          \"type\": \"array\",\n          \"description\": \"Validation errors that must be resolved before confirmation\",\n          \"items\": {\n            \"$ref\": \"#/$defs/ValidationIssue\"\n          }\n        },\n        \"warnings\": {\n          \"type\": \"array\",\n          \"description\": \"Validation warnings that may need attention\",\n          \"items\": {\n            \"$ref\": \"#/$defs/ValidationIssue\"\n          }\n        }\n      }\n    },\n    \"ValidationIssue\": {\n      \"type\": \"object\",\n      \"description\": \"A single validation error or warning\",\n      \"required\"\
  : [\n        \"code\",\n        \"message\"\n      ],\n      \"properties\": {\n        \"code\": {\n          \"type\": \"string\",\n          \"description\": \"Machine-readable validation issue code\"\n        },\n        \"field\": {\n          \"type\": \"string\",\n          \"description\": \"The field that triggered the validation issue\"\n        },\n        \"message\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable description of the issue\"\n        }\n      }\n    },\n    \"Jurisdiction\": {\n      \"type\": \"object\",\n      \"description\": \"A tax jurisdiction supported by Remitian\",\n      \"required\": [\n        \"id\",\n        \"name\",\n        \"country\",\n        \"type\"\n      ],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique jurisdiction identifier\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Display name\
  \ of the tax jurisdiction\"\n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"description\": \"ISO 3166-1 alpha-2 country code\",\n          \"pattern\": \"^[A-Z]{2}$\",\n          \"minLength\": 2,\n          \"maxLength\": 2\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Level of government\",\n          \"enum\": [\n            \"federal\",\n            \"state\",\n            \"provincial\",\n            \"local\"\n          ]\n        },\n        \"taxTypes\": {\n          \"type\": \"array\",\n          \"description\": \"Tax types accepted by this jurisdiction\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"requiredFields\": {\n          \"type\": \"array\",\n          \"description\": \"Fields required for payment submission to this jurisdiction\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"paymentMethods\"\
  : {\n          \"type\": \"array\",\n          \"description\": \"Accepted payment methods\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"active\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this jurisdiction is currently active for payments\"\n        }\n      }\n    },\n    \"Account\": {\n      \"type\": \"object\",\n      \"description\": \"A client account registered for tax payment processing\",\n      \"required\": [\n        \"id\",\n        \"name\",\n        \"email\"\n      ],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique account identifier\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Display name for the client account\",\n          \"minLength\": 1,\n          \"maxLength\": 255\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\"\
  ,\n          \"description\": \"Contact email for the account\"\n        },\n        \"taxIdentifier\": {\n          \"type\": \"string\",\n          \"description\": \"Primary taxpayer identification number\"\n        },\n        \"bankConnections\": {\n          \"type\": \"array\",\n          \"description\": \"Linked and verified bank connections\",\n          \"items\": {\n            \"$ref\": \"#/$defs/BankConnection\"\n          }\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Account verification status\",\n          \"enum\": [\n            \"pending\",\n            \"verified\",\n            \"suspended\"\n          ]\n        },\n        \"createdAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp when the account was created\"\n        }\n      }\n    },\n    \"BankConnection\": {\n      \"type\": \"object\",\n      \"description\": \"A verified bank connection\
  \ linked to a client account\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique bank connection identifier\"\n        },\n        \"institutionName\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the banking institution\"\n        },\n        \"accountLast4\": {\n          \"type\": \"string\",\n          \"description\": \"Last four digits of the bank account number\",\n          \"pattern\": \"^\\\\d{4}$\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Connection verification status\",\n          \"enum\": [\n            \"pending\",\n            \"verified\",\n            \"failed\"\n          ]\n        },\n        \"verifiedAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp when the connection was verified\"\n        }\n      }\n    },\n    \"AuditLogEntry\": {\n      \"\
  type\": \"object\",\n      \"description\": \"A bank-grade audit log entry tracking payment events\",\n      \"required\": [\n        \"id\",\n        \"eventType\",\n        \"timestamp\"\n      ],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique audit log entry identifier\"\n        },\n        \"paymentId\": {\n          \"type\": \"string\",\n          \"description\": \"Associated payment identifier\"\n        },\n        \"accountId\": {\n          \"type\": \"string\",\n          \"description\": \"Associated account identifier\"\n        },\n        \"eventType\": {\n          \"type\": \"string\",\n          \"description\": \"Type of audit event\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable description of the event\"\n        },\n        \"actor\": {\n          \"type\": \"string\",\n          \"description\": \"Identifier of the user or system\
  \ that triggered the event\"\n        },\n        \"ipAddress\": {\n          \"type\": \"string\",\n          \"description\": \"IP address of the request that triggered the event\"\n        },\n        \"timestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the event occurred\"\n        },\n        \"metadata\": {\n          \"type\": \"object\",\n          \"additionalProperties\": true,\n          \"description\": \"Additional context for the audit event\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/remitian/refs/heads/main/json-schema/remitian-payment-schema.json
tags:
- Tax
- Payments
- Fintech
- Accounting
- Webhooks
- Embedded Payments
title: Remitian Tax Payment
---
