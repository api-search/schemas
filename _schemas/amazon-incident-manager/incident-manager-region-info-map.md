---
description: RegionInfoMap schema
layout: schema
name: RegionInfoMap
properties_list: []
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-region-info-map-schema.json
slug: incident-manager-region-info-map
source_filename: incident-manager-region-info-map-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-region-info-map-schema.json\",\n  \"title\": \"RegionInfoMap\",\n  \"description\": \"RegionInfoMap schema\",\n  \"type\": \"object\",\n  \"additionalProperties\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"status\",\n      \"statusUpdateDateTime\"\n    ],\n    \"properties\": {\n      \"sseKmsKeyId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/SseKmsKey\"\n          },\n          {\n            \"description\": \"The ID of the KMS key used to encrypt the data in this Amazon Web Services Region.\"\n          }\n        ]\n      },\n      \"status\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/RegionStatus\"\n          },\n          {\n            \"description\": \"The status of the Amazon\
  \ Web Services Region in the replication set.\"\n          }\n        ]\n      },\n      \"statusMessage\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/String\"\n          },\n          {\n            \"description\": \"Information displayed about the status of the Amazon Web Services Region.\"\n          }\n        ]\n      },\n      \"statusUpdateDateTime\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Timestamp\"\n          },\n          {\n            \"description\": \"The most recent date and time that Incident Manager updated the Amazon Web Services Region's status.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Information about a Amazon Web Services Region in your replication set.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-region-info-map-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: RegionInfoMap
---
