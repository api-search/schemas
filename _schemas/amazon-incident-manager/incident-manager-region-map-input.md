---
description: RegionMapInput schema
layout: schema
name: RegionMapInput
properties_list: []
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-region-map-input-schema.json
slug: incident-manager-region-map-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-region-map-input-schema.json\",\n  \"title\": \"RegionMapInput\",\n  \"description\": \"RegionMapInput schema\",\n  \"type\": \"object\",\n  \"additionalProperties\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"sseKmsKeyId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/SseKmsKey\"\n          },\n          {\n            \"description\": \"The KMS key used to encrypt the data in your replication set.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"The mapping between a Amazon Web Services Region and the key that's used to encrypt the data.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-region-map-input-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: RegionMapInput
---
