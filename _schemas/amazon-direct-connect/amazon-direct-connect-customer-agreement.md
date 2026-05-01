---
description: The name and status of a customer agreement.
layout: schema
name: CustomerAgreement
properties_list:
- description: ''
  name: agreementName
  type: object
- description: ''
  name: status
  type: object
provider_name: Amazon Direct Connect
provider_slug: amazon-direct-connect
schema_file: json-schema/amazon-direct-connect-customer-agreement-schema.json
slug: amazon-direct-connect-customer-agreement
source_filename: amazon-direct-connect-customer-agreement-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-direct-connect/refs/heads/main/json-schema/amazon-direct-connect-customer-agreement-schema.json\",\n  \"title\": \"CustomerAgreement\",\n  \"description\": \"The name and status of a customer agreement.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"agreementName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AgreementName\"\n        },\n        {\n          \"description\": \"The name of the agreement.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Status\"\n        },\n        {\n          \"description\": \"The status of the customer agreement. This will be either <code>signed</code> or <code>unsigned</code> \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-direct-connect/refs/heads/main/json-schema/amazon-direct-connect-customer-agreement-schema.json
tags:
- Dedicated Connection
- Direct Connect
- Hybrid Cloud
- Networking
title: CustomerAgreement
---
