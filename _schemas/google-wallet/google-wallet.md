---
description: JSON Schema for Google Wallet API pass class and object definitions.
layout: schema
name: Google Wallet API Schema
properties_list: []
provider_name: Google Wallet
provider_slug: google-wallet
schema_file: json-schema/google-wallet.json
slug: google-wallet
source_filename: google-wallet.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-wallet/refs/heads/main/json-schema/google-wallet.json\",\n  \"title\": \"Google Wallet API Schema\",\n  \"description\": \"JSON Schema for Google Wallet API pass class and object definitions.\",\n  \"type\": \"object\",\n  \"$defs\": {\n    \"GenericClass\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the class.\"\n        },\n        \"classTemplateInfo\": {\n          \"type\": \"object\",\n          \"description\": \"Template information for the class.\"\n        },\n        \"imageModulesData\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\"\n          }\n        },\n        \"textModulesData\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\":\
  \ \"object\"\n          }\n        },\n        \"multipleDevicesAndHoldersAllowedStatus\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"GenericObject\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the object.\"\n        },\n        \"classId\": {\n          \"type\": \"string\",\n          \"description\": \"The class this object belongs to.\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"enum\": [\"ACTIVE\", \"COMPLETED\", \"EXPIRED\", \"INACTIVE\"],\n          \"description\": \"State of the pass.\"\n        },\n        \"barcode\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"type\": {\n              \"type\": \"string\"\n            },\n            \"value\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"header\": {\n          \"type\"\
  : \"object\",\n          \"properties\": {\n            \"defaultValue\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"language\": {\n                  \"type\": \"string\"\n                },\n                \"value\": {\n                  \"type\": \"string\"\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"EventTicketClass\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"eventName\": {\n          \"type\": \"object\"\n        },\n        \"venue\": {\n          \"type\": \"object\"\n        },\n        \"dateTime\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"start\": { \"type\": \"string\" },\n            \"end\": { \"type\": \"string\" }\n          }\n        },\n        \"issuerName\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"LoyaltyClass\"\
  : {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"issuerName\": {\n          \"type\": \"string\"\n        },\n        \"programName\": {\n          \"type\": \"string\"\n        },\n        \"reviewStatus\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-wallet/refs/heads/main/json-schema/google-wallet.json
tags:
- Digital Wallet
- Google Wallet
- Loyalty Cards
- Mobile Payments
- Passes
- Tickets
title: Google Wallet API Schema
---
