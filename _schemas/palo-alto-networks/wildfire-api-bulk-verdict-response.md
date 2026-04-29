---
description: WildFire bulk verdict results for multiple hash queries.
layout: schema
name: BulkVerdictResponse
properties_list:
- description: ''
  name: get-verdicts-info
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/wildfire-api-bulk-verdict-response-schema.json
slug: wildfire-api-bulk-verdict-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BulkVerdictResponse\",\n  \"description\": \"WildFire bulk verdict results for multiple hash queries.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/wildfire-api-bulk-verdict-response-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"get-verdicts-info\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"entry\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"md5\": {\n                \"type\": \"string\"\n              },\n              \"sha256\": {\n                \"type\": \"string\"\n              },\n              \"verdict\": {\n                \"type\": \"integer\"\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/wildfire-api-bulk-verdict-response-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: BulkVerdictResponse
---
