---
description: Response returned after successfully submitting a file, URL, or link.
layout: schema
name: SubmitResponse
properties_list:
- description: ''
  name: upload-file-info
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/wildfire-api-submit-response-schema.json
slug: wildfire-api-submit-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SubmitResponse\",\n  \"description\": \"Response returned after successfully submitting a file, URL, or link.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/wildfire-api-submit-response-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"upload-file-info\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"filename\": {\n          \"type\": \"string\",\n          \"description\": \"Original filename of the submitted file.\"\n        },\n        \"filetype\": {\n          \"type\": \"string\",\n          \"description\": \"Detected file type.\"\n        },\n        \"fileurl\": {\n          \"type\": \"string\",\n          \"description\": \"URL of the submitted link or URL sample.\"\n        },\n        \"md5\": {\n          \"type\": \"string\",\n          \"description\": \"MD5 hash of the submitted\
  \ file.\"\n        },\n        \"sha256\": {\n          \"type\": \"string\",\n          \"description\": \"SHA-256 hash of the submitted file.\"\n        },\n        \"size\": {\n          \"type\": \"integer\",\n          \"description\": \"File size in bytes.\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"description\": \"Submitted URL value.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/wildfire-api-submit-response-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: SubmitResponse
---
