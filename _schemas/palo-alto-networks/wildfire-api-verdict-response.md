---
description: WildFire verdict result for a single file hash query.
layout: schema
name: VerdictResponse
properties_list:
- description: ''
  name: get-verdict-info
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/wildfire-api-verdict-response-schema.json
slug: wildfire-api-verdict-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VerdictResponse\",\n  \"description\": \"WildFire verdict result for a single file hash query.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/wildfire-api-verdict-response-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"get-verdict-info\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"md5\": {\n          \"type\": \"string\",\n          \"description\": \"MD5 hash of the queried file.\"\n        },\n        \"sha256\": {\n          \"type\": \"string\",\n          \"description\": \"SHA-256 hash of the queried file.\"\n        },\n        \"verdict\": {\n          \"type\": \"integer\",\n          \"description\": \"Verdict code: 0 (benign), 1 (malware), 2 (grayware), 4 (phishing), -100 (pending), -101 (error), -102 (unknown), -103 (invalid hash).\",\n          \"enum\": [\n           \
  \ 0,\n            1,\n            2,\n            4,\n            -100,\n            -101,\n            -102,\n            -103\n          ]\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/wildfire-api-verdict-response-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: VerdictResponse
---
