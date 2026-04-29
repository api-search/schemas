---
description: Represents the metadata of an offering transaction.
layout: schema
name: OfferingTransaction
properties_list:
- description: ''
  name: offeringStatus
  type: object
- description: ''
  name: transactionId
  type: object
- description: ''
  name: offeringPromotionId
  type: object
- description: ''
  name: createdOn
  type: object
- description: ''
  name: cost
  type: object
provider_name: Amazon Device Farm
provider_slug: amazon-device-farm
schema_file: json-schema/amazon-device-farm-offering-transaction-schema.json
slug: amazon-device-farm-offering-transaction
source_filename: amazon-device-farm-offering-transaction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/json-schema/amazon-device-farm-offering-transaction-schema.json\",\n  \"title\": \"OfferingTransaction\",\n  \"description\": \"Represents the metadata of an offering transaction.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"offeringStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OfferingStatus\"\n        },\n        {\n          \"description\": \"The status of an offering transaction.\"\n        }\n      ]\n    },\n    \"transactionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TransactionIdentifier\"\n        },\n        {\n          \"description\": \"The transaction ID of the offering transaction.\"\n        }\n      ]\n    },\n    \"offeringPromotionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OfferingPromotionIdentifier\"\
  \n        },\n        {\n          \"description\": \"The ID that corresponds to a device offering promotion.\"\n        }\n      ]\n    },\n    \"createdOn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"The date on which an offering transaction was created.\"\n        }\n      ]\n    },\n    \"cost\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MonetaryAmount\"\n        },\n        {\n          \"description\": \"The cost of an offering transaction.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/json-schema/amazon-device-farm-offering-transaction-schema.json
tags:
- Application Testing
- AWS
- Device Testing
- Mobile Testing
- Quality Assurance
title: OfferingTransaction
---
