---
description: Defines the Amazon Web Services Region and KMS key to add to the replication set.
layout: schema
name: AddRegionAction
properties_list:
- description: ''
  name: regionName
  type: object
- description: ''
  name: sseKmsKeyId
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-add-region-action-schema.json
slug: incident-manager-add-region-action
source_filename: incident-manager-add-region-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-add-region-action-schema.json\",\n  \"title\": \"AddRegionAction\",\n  \"description\": \"Defines the Amazon Web Services Region and KMS key to add to the replication set. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"regionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RegionName\"\n        },\n        {\n          \"description\": \"The Amazon Web Services Region name to add to the replication set.\"\n        }\n      ]\n    },\n    \"sseKmsKeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SseKmsKey\"\n        },\n        {\n          \"description\": \"The KMS key ID to use to encrypt your replication set.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"regionName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-add-region-action-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: AddRegionAction
---
