---
description: Information identifying the person picking up the device.
layout: schema
name: PickupDetails
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: PhoneNumber
  type: object
- description: ''
  name: Email
  type: object
- description: ''
  name: IdentificationNumber
  type: object
- description: ''
  name: IdentificationExpirationDate
  type: object
- description: ''
  name: IdentificationIssuingOrg
  type: object
- description: ''
  name: DevicePickupId
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-pickup-details-schema.json
slug: amazon-snow-family-pickup-details
source_filename: amazon-snow-family-pickup-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-pickup-details-schema.json\",\n  \"title\": \"PickupDetails\",\n  \"description\": \"Information identifying the person picking up the device.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the person picking up the device.\"\n        }\n      ]\n    },\n    \"PhoneNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PhoneNumber\"\n        },\n        {\n          \"description\": \"The phone number of the person picking up the device.\"\n        }\n      ]\n    },\n    \"Email\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Email\"\n        },\n    \
  \    {\n          \"description\": \"The email address of the person picking up the device.\"\n        }\n      ]\n    },\n    \"IdentificationNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The number on the credential identifying the person picking up the device.\"\n        }\n      ]\n    },\n    \"IdentificationExpirationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"Expiration date of the credential identifying the person picking up the device.\"\n        }\n      ]\n    },\n    \"IdentificationIssuingOrg\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Organization that issued the credential identifying the person picking up the device.\"\n        }\n      ]\n    },\n    \"DevicePickupId\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DevicePickupId\"\n        },\n        {\n          \"description\": \"The unique ID for a device that will be picked up.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-pickup-details-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: PickupDetails
---
