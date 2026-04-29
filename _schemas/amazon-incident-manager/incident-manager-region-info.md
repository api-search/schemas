---
description: Information about a Amazon Web Services Region in your replication set.
layout: schema
name: RegionInfo
properties_list:
- description: ''
  name: sseKmsKeyId
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: statusMessage
  type: object
- description: ''
  name: statusUpdateDateTime
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-region-info-schema.json
slug: incident-manager-region-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-region-info-schema.json\",\n  \"title\": \"RegionInfo\",\n  \"description\": \"Information about a Amazon Web Services Region in your replication set.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sseKmsKeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SseKmsKey\"\n        },\n        {\n          \"description\": \"The ID of the KMS key used to encrypt the data in this Amazon Web Services Region.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RegionStatus\"\n        },\n        {\n          \"description\": \"The status of the Amazon Web Services Region in the replication set.\"\n        }\n      ]\n    },\n    \"statusMessage\": {\n      \"allOf\": [\n  \
  \      {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Information displayed about the status of the Amazon Web Services Region.\"\n        }\n      ]\n    },\n    \"statusUpdateDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The most recent date and time that Incident Manager updated the Amazon Web Services Region's status.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"status\",\n    \"statusUpdateDateTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-region-info-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: RegionInfo
---
