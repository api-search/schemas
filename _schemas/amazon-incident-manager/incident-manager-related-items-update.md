---
description: Details about the related item you're adding.
layout: schema
name: RelatedItemsUpdate
properties_list:
- description: ''
  name: itemToAdd
  type: object
- description: ''
  name: itemToRemove
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-related-items-update-schema.json
slug: incident-manager-related-items-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-related-items-update-schema.json\",\n  \"title\": \"RelatedItemsUpdate\",\n  \"description\": \"Details about the related item you're adding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"itemToAdd\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RelatedItem\"\n        },\n        {\n          \"description\": \"Details about the related item you're adding.\"\n        }\n      ]\n    },\n    \"itemToRemove\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ItemIdentifier\"\n        },\n        {\n          \"description\": \"Details about the related item you're deleting.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-related-items-update-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: RelatedItemsUpdate
---
