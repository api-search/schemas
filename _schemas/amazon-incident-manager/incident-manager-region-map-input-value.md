---
description: The mapping between a Amazon Web Services Region and the key that's used to encrypt the data.
layout: schema
name: RegionMapInputValue
properties_list:
- description: ''
  name: sseKmsKeyId
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-region-map-input-value-schema.json
slug: incident-manager-region-map-input-value
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-region-map-input-value-schema.json\",\n  \"title\": \"RegionMapInputValue\",\n  \"description\": \"The mapping between a Amazon Web Services Region and the key that's used to encrypt the data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sseKmsKeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SseKmsKey\"\n        },\n        {\n          \"description\": \"The KMS key used to encrypt the data in your replication set.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-region-map-input-value-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: RegionMapInputValue
---
