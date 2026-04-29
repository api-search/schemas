---
description: JSON Schema for an ACORD NGDS insurance claim object, representing a first notice of loss through claim settlement.
layout: schema
name: ACORD Claim
properties_list:
- description: Unique internal claim identifier
  name: claimId
  type: string
- description: Carrier-assigned claim number
  name: claimNumber
  type: string
- description: Reference to the associated policy
  name: policyId
  type: string
- description: ''
  name: policyNumber
  type: string
- description: ''
  name: status
  type: string
- description: Date the loss or incident occurred
  name: lossDate
  type: string
- description: Date the claim was reported
  name: reportedDate
  type: string
- description: Narrative description of the loss
  name: lossDescription
  type: string
- description: Type of loss event
  name: lossType
  type: string
- description: ''
  name: lossLocation
  type: object
- description: ''
  name: claimant
  type: object
- description: ''
  name: adjuster
  type: object
- description: Current reserve amount set for this claim
  name: reserveAmount
  type: number
- description: Total amount paid on this claim to date
  name: paidAmount
  type: number
- description: ''
  name: currency
  type: string
- description: ''
  name: payments
  type: array
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
provider_name: ACORD
provider_slug: acord
schema_file: json-schema/acord-claim-schema.json
slug: acord-claim
source_filename: acord-claim-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acord/refs/heads/main/json-schema/acord-claim-schema.json\",\n  \"title\": \"ACORD Claim\",\n  \"description\": \"JSON Schema for an ACORD NGDS insurance claim object, representing a first notice of loss through claim settlement.\",\n  \"type\": \"object\",\n  \"required\": [\"claimId\", \"claimNumber\", \"policyId\", \"status\", \"lossDate\"],\n  \"properties\": {\n    \"claimId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique internal claim identifier\"\n    },\n    \"claimNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Carrier-assigned claim number\"\n    },\n    \"policyId\": {\n      \"type\": \"string\",\n      \"description\": \"Reference to the associated policy\"\n    },\n    \"policyNumber\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"Open\"\
  , \"Closed\", \"Pending\", \"Denied\", \"Paid\"]\n    },\n    \"lossDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the loss or incident occurred\"\n    },\n    \"reportedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the claim was reported\"\n    },\n    \"lossDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Narrative description of the loss\"\n    },\n    \"lossType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of loss event\",\n      \"enum\": [\"Collision\", \"Theft\", \"Fire\", \"Water\", \"Wind\", \"Liability\", \"Medical\", \"Other\"]\n    },\n    \"lossLocation\": {\n      \"$ref\": \"#/$defs/Address\"\n    },\n    \"claimant\": {\n      \"$ref\": \"#/$defs/Party\"\n    },\n    \"adjuster\": {\n      \"$ref\": \"#/$defs/Party\"\n    },\n    \"reserveAmount\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"description\"\
  : \"Current reserve amount set for this claim\"\n    },\n    \"paidAmount\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"description\": \"Total amount paid on this claim to date\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"default\": \"USD\"\n    },\n    \"payments\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ClaimPayment\"\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"$defs\": {\n    \"Party\": {\n      \"type\": \"object\",\n      \"required\": [\"partyType\"],\n      \"properties\": {\n        \"partyId\": {\n          \"type\": \"string\"\n        },\n        \"partyType\": {\n          \"type\": \"string\",\n          \"enum\": [\"Insured\", \"Claimant\", \"Agent\", \"Broker\", \"Carrier\", \"Adjuster\"]\n        },\n        \"firstName\":\
  \ {\n          \"type\": \"string\"\n        },\n        \"lastName\": {\n          \"type\": \"string\"\n        },\n        \"organizationName\": {\n          \"type\": \"string\"\n        },\n        \"address\": {\n          \"$ref\": \"#/$defs/Address\"\n        }\n      }\n    },\n    \"ClaimPayment\": {\n      \"type\": \"object\",\n      \"required\": [\"paymentId\", \"amount\", \"paymentDate\"],\n      \"properties\": {\n        \"paymentId\": {\n          \"type\": \"string\"\n        },\n        \"amount\": {\n          \"type\": \"number\",\n          \"minimum\": 0\n        },\n        \"paymentDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\"\n        },\n        \"paymentType\": {\n          \"type\": \"string\",\n          \"enum\": [\"Check\", \"EFT\", \"Wire\"]\n        },\n        \"coverageType\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"Address\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"\
  street1\": {\"type\": \"string\"},\n        \"street2\": {\"type\": \"string\"},\n        \"city\": {\"type\": \"string\"},\n        \"state\": {\"type\": \"string\"},\n        \"postalCode\": {\"type\": \"string\"},\n        \"country\": {\"type\": \"string\", \"default\": \"US\"}\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acord/refs/heads/main/json-schema/acord-claim-schema.json
tags:
- Claims
- Insurance
- Policy
- Standards
- Underwriting
title: ACORD Claim
---
