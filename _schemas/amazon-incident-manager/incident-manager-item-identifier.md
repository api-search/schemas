---
description: Details and type of a related item.
layout: schema
name: ItemIdentifier
properties_list:
- description: ''
  name: type
  type: object
- description: ''
  name: value
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-item-identifier-schema.json
slug: incident-manager-item-identifier
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-item-identifier-schema.json\",\n  \"title\": \"ItemIdentifier\",\n  \"description\": \"Details and type of a related item.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ItemType\"\n        },\n        {\n          \"description\": \"The type of related item. \"\n        }\n      ]\n    },\n    \"value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ItemValue\"\n        },\n        {\n          \"description\": \"Details about the related item.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-item-identifier-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: ItemIdentifier
---
